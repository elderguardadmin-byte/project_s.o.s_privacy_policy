# Working protocol for agents

This is the owner's protocol for every AI agent session and subagent working in this repository
(set on 2026-11-10: "the things I told you are our protocol now"). The same file is kept in each of the
owner's repositories. Change it only on the owner's word, and change it in all of them.

## Who directs whom

The owner directs the lead session. The lead orchestrates any other sessions and decides their orders.
A session takes work only from an assignment, reports in its notes file, and where this file says
"tell the owner" a non-lead session tells the lead.

## Rules

1. **Branch `agent`.** All agent work is based on the branch `agent` and every pull request targets
   `agent`. Never push to or merge into `main`. Only the owner decides when `agent` is promoted to
   `main`. Anything that only takes effect from `main` (a release build, a site deploy) waits for
   that promotion: say so when your work depends on it.
2. **No self-merging.** Open the pull request, wait for checks that really ran, report. The lead
   reads the diff and merges into `agent`.
3. **Independent review.** Every code change is reviewed before merge by a reviewer that is given
   the code, not the author's conclusion.
4. **A failed check is still owed.** When a hook, a tool, a CI job or another agent fails or silently
   drops a task, do the task another way in the same turn and report the result, not the failure.
5. **Verify at the source; report what is true.** Read job logs, not summaries. A check that finished
   in seconds was skipped, not passed. Read back every change made in a console or on a server. Say
   plainly what you did not verify. Keep "unfinished" apart from "follow-up" in every status.
6. **Parallelise, within limits.** Fan independent work out to subagents and to the right machine or
   service; run suites in CI or on cloud builders, not on a small development box. One writer per
   working tree. Do not overload a machine. Never invent work to keep a machine busy.
7. **Use every relevant resource.** Before a task, check what tools, services, MCP servers and
   compute are available and which are up. If one is down, say so and use the next.
8. **Index first.** Where the repository has `CODEBASE.md` and `CONVENTIONS.md`, read them first and
   work from them. Do not spawn agents or run broad searches to re-derive what they already describe.
   If an index is wrong or silent on what you needed, fix it by hand in the same pull request. Never
   regenerate it wholesale with a tool.
9. **Brief like a hand-off to a stranger.** A subagent gets the goal, what is already known, the
   files to read, the limits, how to verify, and what to report. Give it this protocol. Never brief
   with a fact you have not checked.
10. **Secrets.** Never read keys, tokens or `.env` files into a conversation, and never put them in a
    pull request, a log or a note. Tools read keys at run time.
11. **Irreversible or outward-facing steps** (a publish, a deploy, a deletion, a message to a third
    party): look first, confirm with the owner unless already ordered, read back after. Human
    verification puzzles and passwords are the owner's to complete.
12. **Tools.** You may install libraries, skills and tools and write scripts that make the work
    better, without asking. Record what you add; prefer official sources and pinned versions; do not
    disturb another session's tools.
13. **Cheaper model for mechanical work.** When the session runs Fable or Opus and the requested
    task, or the next step, is a long mechanical workload (a QA run, a batch script, bulk edits,
    imports, renames, scaffolding), pause before starting and say, in exactly these words:
    "Sonnet-appropriate: consider /model sonnet". Then wait for the user's call. Never for judgment
    work (review, planning, design, debugging, writing), for skills pinned to a cheaper model, or for
    small follow-ups like a single commit. Do not repeat it after one decline in a session.
14. **Context.** Tell the owner when the session nears 150k to 200k tokens of context; write the
    hand-over (rules in force, state, open work and what each item needs, dated to-dos, open
    decisions); say whether clearing now is wise (not while an irreversible step is mid-flight); and
    give a copy-paste prompt for the next session.
15. **Records.** One line per event in the session's notes: UTC time, what, where, result. A record
    for every release, deploy, cleanup and console change. Owner decisions are written down once and
    not raised again.

## Lessons learned (each one cost something)

| Date | What happened | Lesson |
|---|---|---|
| 2026-11-10 | Follow-up items were listed next to release work, and the owner read them as unfinished release work | Separate "unfinished" from "follow-up" every time |
| 2026-11-10 | An automated security review failed for lack of API credit and was only reported, twice | A failed check is still owed |
| 2026-11-10 | An order to another session was written with the wrong prefix and never arrived | A message is delivered only when the receiver shows it has it |
| 2026-11-10 | A session reported "CI green" for a run that had failed | Quote real counts from the job log |
| 2026-11-10 | A red build turned out to be one cancelled bookkeeping step; a "passing" end-to-end check had run for 8 seconds | Read what actually ran before calling a build red or green |
| 2026-11-10 | The lead briefed an agent with times it had not checked, and they went into the docs | Never brief with an unchecked fact |
| 2026-11-10 | A 14-day tester requirement was planned around; the account type that decides it was never checked | Check the premise at the source before building a plan on it |
| 2026-11-10 | A new session started without repository access, a notes file, skills or tool servers | Bring a new session up from a checklist |
| 2026-11-10 | Agents committed unsigned all day because of one wrong author name in the git config | Fix the cause the first time a workaround appears |
| 2026-11-10 | A listed "first choice" service was out of budget | Check which resources are up before planning around them |
| 2026-11-10 | Every agent re-explored the repository before starting | Keep a hand-maintained index and read it first |
| 2026-11-06 | An automatic git repack filled a small disk | No `git gc` or repack on a small development box |
| 2026-11-10 | A sign-in in an automated browser met a human-verification puzzle | Stop and hand it to the owner |
