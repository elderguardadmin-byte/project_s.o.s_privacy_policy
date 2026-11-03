# Privacy policy

Project S.O.S, by Upton Software Ltd. Liability Company

Effective date: 3 November 2026

This policy covers the Project S.O.S app on iPhone, iPad and Android. It says the same as the "Privacy and terms" screen inside the app, with more detail. A copy is published at https://elderguardadmin-byte.github.io/project_s.o.s_privacy_policy/.

## The short version

The app sends nothing to Upton Software Ltd. Liability Company. The company has no servers, no accounts, no analytics and no ads. The company never sees your alerts, your people, your recordings or your location.

What you put in the app stays on your device, encrypted. It leaves your device only when you send it, or when a person you allowed asks for your location. It goes only to the people and services you choose.

## Who makes the app

Project S.O.S is made by Upton Software Ltd. Liability Company, a limited liability company organized in the State of Georgia, USA, at 8735 Dunwoody Place, Atlanta, GA 30350, USA.

## What Upton Software Ltd. Liability Company holds about you

The app does not send Upton Software Ltd. Liability Company any personal data. So for the data you keep in the app, the company is not a "controller" under data protection law. You decide what goes in it and who it goes to.

Upton Software Ltd. Liability Company holds personal data in only two cases:

- **If you email Upton Software Ltd. Liability Company.** The company gets your email address and what you write. It uses them only to answer you and to keep a record of what you and the company agreed. Its lawful basis is its legitimate interest in giving support. It keeps support emails for up to two years after the last message, then deletes them, unless it needs them longer for a legal claim.
- **Store reports.** Apple and Google collect data when you buy or use the app, under their own privacy policies. They give Upton Software Ltd. Liability Company sales reports, which can show the country of each purchase, and, if you agreed to share them with developers, crash reports. These do not include your alerts, contacts or location. The company uses them only to keep track of sales and fix bugs.

Upton Software Ltd. Liability Company is the controller for this data. The company does not sell it or share it, except where the law requires.

The company is based in the United States, so support emails are kept and answered there. Please do not put health details or other sensitive information in a support email. The company does not need them to help you.

## What stays on your device

Everything you put in the app stays on your device. That includes your name, your phone number, your people and groups, your emergency types, your health details if you add them, your settings, your recordings and your alert history. It also includes:

- notes you write about an encounter (a name, badge or ID number, agency, vehicle plate, your own text and, if location is allowed, where the phone was), each signed with your own key when you save it;
- answers your people send to your alerts ("On my way", "I'm calling you", "I can't come") and the answers you send to theirs;
- trips your people share with you, kept until 24 hours after the time they expected to arrive;
- what each person may ask your phone for (both off by default), the requests you sent and the notices about requests you received;
- sound recordings you start without an alert, and what dashcam mode keeps;
- the person whose calls are answered during an alert (Android), the car you chose for dashcam mode, your volume button pattern and your home screen icon choice.

The alert history is a log of the alerts you sent and received: the emergency type, the times, who it went to or came from, whether it was delivered and seen, the answers, the location trail, any recordings and your own notes. Sound recordings made without an alert are listed there too, marked "No alert was sent". It is kept for 1 year unless you change that in Settings, Data, Alert history (forever, 1 year, 90 days or 30 days). Alerts that still have recordings are kept until you delete them.

Quick triggers are the one exception to "encrypted by the app". So that the widget, the quick settings tile, the app icon shortcut, Siri or Google Assistant and your watch can show the right words without opening the app's database, the app keeps a small list in the device's own app storage: which quick triggers are on and which emergency type each sends, and the names of your emergency types only while Siri or Google Assistant is on or you chose "Show the emergency name". It holds no people, phone numbers, messages or locations. It is protected by your device's own encryption, not by the app's key, and it is not included in device or cloud backups. On Android, "Start dashcam in my car" keeps the Bluetooth name of the car you chose in the same kind of app storage, so the phone can offer dashcam mode when the car connects while the app is closed. By default the widget, the lock screen, the tile and the app icon shortcut just say "Quick alert", so someone holding your phone cannot see what your emergency types are. You can turn each quick trigger off, or choose to show the names, in Settings, Triggers, Quick triggers.

It is all stored encrypted. The database is locked with a random key held in your device's secure keystore (the Keychain on iPhone and iPad, the Keystore on Android). Each recording is encrypted with its own key. A recording is written in short pieces; each piece is encrypted as soon as it is finished and the unencrypted copy is deleted. If the app is stopped while recording, the unfinished piece is encrypted and filed with its own alert the next time the app opens.

The app's data is not included in your phone's own backups. On Android the app turns off Android backup and device-to-device transfer. On iPhone and iPad its recordings, including any unfinished piece, and the live backup's working copies and locked key file are kept out of iCloud and computer backups. To move your people, settings and history to a new phone, use the app's own backup (below), which is locked with your passphrase.

If you set safety PINs (an all clear PIN and a duress PIN), the app keeps only a salted Argon2id hash of each one in the same secure keystore, never the PIN itself. When you use the duress PIN, the app looks as if your alert ended, but keeps sending encrypted app messages with your location to your people, telling them you may be under duress. It sends a text message too only if you turned that on. This record of the alert is hidden from this phone's alert history until you enter your all clear PIN.

As each part of a recording is saved, the app takes its SHA-256 fingerprint and signs it with your own key, in a list kept encrypted next to the recording. This lets you show later that a file has not been changed since your phone signed it. Notes you write are signed the same way. It does not prove what happened, and nothing about it is sent to Upton Software Ltd. Liability Company or anyone else.

### Recording without an alert

"Record sound only" on the SOS screen records sound with the microphone without sending an alert. Nobody is told. Dashcam mode records in short pieces (with the camera, or sound only) and keeps only the last few minutes you chose; older pieces are deleted as new ones are made, and turning it off deletes what it kept. Both are encrypted on your device in the same way as alert recordings and are never uploaded by themselves. If you press SOS while dashcam mode is on, the minutes before the press are kept with that alert's recordings. If the app closes while dashcam mode is recording, what it kept is filed in your alert history the next time the app opens, for you to keep or delete. On Android a notification shows while either one records. On iPhone and iPad the system shows its own microphone or camera indicator.

### Panic lock and panic wipe

Panic lock makes the app look new and empty until you enter your unlock PIN. Nothing is deleted. Panic wipe deletes the keys that unlock the app's data from the Keychain or Keystore, then deletes the app's files, when you type your wipe PIN. After that, nothing the app kept on that phone can be read. Phone storage may keep pieces of deleted files for a while, but without the keys they cannot be read. The app keeps only a salted Argon2id hash of these PINs, like your other safety PINs.

### Answering calls during an alert (Android)

If you turn on "Answer calls during an alert" (off by default, Android 10 and newer), a call from the one person you chose is answered by itself while an alert is on, and the speaker is turned on. That person can then hear what is happening near your phone. For this the app needs to answer phone calls, to be your phone's caller ID and spam app, and Contacts. It uses these only to see the number of an incoming call. The number is compared on your device. It is never saved or sent. The app never reads, copies or stores your contacts list, and it never blocks, silences or hides a call. It does nothing when no alert is on, or while an alert you ended with your duress PIN is still running. The answered call shows in your call history as normal.

### Fake call and blank screen

The fake call and blank screen are shown by the app on your phone. They send nothing and record nothing.

## What leaves your device, and who gets it

Data leaves your device only when you send an alert, a note, a trip, an answer or a request, stream, upload or share something, or when a person you allowed asks for your location. It goes only to the people and services you chose. Upton Software Ltd. Liability Company is not one of them.

An alert holds what you set up for that emergency type. That can include your name, the emergency type, your location, your phone's battery level, a check-in timer note and the time it was due, a note that you may be under duress, a link to your live stream and any details you filled in, such as medical notes.

Other things can go to your people, in the same two ways, when you choose them:

- **Notes during an alert.** If "Also send to my people" is on when you save a note (it is on by default during an alert), the note goes as an update to the alert, by text and by app message.
- **Live location.** During an alert, "Share live location" sends your location to the alert's people every so often. Each emergency type sets whether it starts on; you can turn it on or off during the alert.
- **"Tell them I'm safe".** If an alert was left on, this sends an end message by text and app message, with your name, your phone number if you added one, the alert's title and the last location the alert had.
- **Trips.** With a check-in timer you can "Tell them now": where you are going, when you expect to arrive, your note and, if that emergency type sends location, where you are. It goes by app message, and by text to people who do not have the app (with a maps link if location is included). They get another message when you extend, check in or cancel.
- **Answers.** When someone sends you an alert, you can answer "On my way", "I'm calling you" or "I can't come". The answer goes to them by app message. "On my way" also goes by text if they have a phone number.
- **Requests.** You can let a person ask your phone where you are, or ask it to record. Both are off by default and set for each person. Requests come only by app message, never by text. If you allowed it, your phone answers a location request by sending your location to that person by app message. A request to record starts your alert's recording only while an alert is running; otherwise the app asks you, and nothing records without you. Each time, your phone shows you a notice and a notification, except while an alert you ended with your duress PIN is still running.

### Text messages

When you send an alert, the app opens your messaging app with a text already written. You tap Send.

The text goes from your own phone number through your mobile carrier, like any other text. Text messages are not encrypted. Your carrier, and anyone who can read the recipient's phone, can read it. Your carrier's own privacy policy applies.

### Email and phone calls

Some people, such as your lawyer, may not use the app. For them you can add an email address and phone numbers.

Email: the app opens your own mail app with a message already written. You tap Send. The email goes through your own email provider, like any other email you send, and their privacy policy applies. Email is usually not end-to-end encrypted. The app has no mail server, and nothing goes through Upton Software Ltd. Liability Company.

Calls: a call button opens your phone app with the number filled in. You place the call. The app never calls anyone by itself.

### Your lawyer

You can mark a person as "My lawyer" and add their name, firm, phone numbers, email and a note, such as where they practise and their registration number. This stays on your device, encrypted, like your other people. For the emergency types you choose, your lawyer can be sent a shorter message by text and email. You can change what it says. Your lawyer gets it only when you tap Send.

Upton Software Ltd. Liability Company does not supply, check or recommend lawyers. "Find a lawyer" only links to official regulators and government legal aid websites. Each link opens in your own web browser, and that website's own privacy policy applies. Before opening a link, the app checks your phone can reach that website. Nothing about you is sent to the company.

### Your rights at a traffic stop

When "Getting pulled over" is the emergency type, the app shows a "Your rights at a traffic stop" card. It links only to official government and court pages for your area. The app does not summarise the law.

To pick the area, the app uses one of these, in this order: an area you chose in Settings, your location, or your phone's language and region settings. If you allowed location, the app reads your phone's last known location when the card is shown and looks up the area in a map file built into the app. This happens on your device. Your location is not saved for this and is not sent anywhere. If you did not allow location, the app does not ask for it here. The area you choose in Settings is kept, encrypted, with your other settings.

Each link opens in your own web browser, never inside the app, and that website's own privacy policy applies. Before opening a link, the app checks your phone can reach that website by looking up its address. That lookup goes to your network's DNS service, like any website you visit. Nothing about you is sent to Upton Software Ltd. Liability Company.

### Encrypted app messages

Alerts to people who also use the app are sent as encrypted app messages as well. While an alert is running, the app also sends location updates to the same people this way. Answers, trips, requests and their replies, and "Tell them I'm safe" use the same encrypted app messages. Messages are encrypted on your device so that only the person you sent them to can open them. They travel through public relays on the Nostr network.

Relays are run by third parties, not by Upton Software Ltd. Liability Company. The company has no contract with them. You can see and change the list of relays in the app's settings.

A relay cannot read your message. It cannot see who sent it, the emergency type, your location or your details. A relay can see:

- your IP address, unless you use a VPN or Tor
- the recipient's public key (their app code)
- a random one-time key used only for that message
- roughly when the message was sent, and its padded size
- that several messages came from the same IP address at the same time, which can link the people who got one alert

The app also checks the relays for alerts sent to you. When it does, the relays see your IP address and your own public key.

Each relay operator has their own policies, and some keep messages for a time. Relays can be in any country.

### Nearby delivery (Bluetooth)

Nearby delivery is off until you turn it on. When it is on, your encrypted app message is also passed over Bluetooth to phones close by that run the app. This helps when you have no signal. A phone close by can hand it to your people directly, pass it to another phone, or send it on to the relays once it has signal. It is the same sealed message the relays get, so those phones cannot read it either. They can see the recipient's public key, roughly when it was sent, and that a phone running the app is close to them. The app advertises only a fixed code that says it is Project S.O.S, never your name.

Carrying other people's alerts is a separate choice, also off until you agree to it. If you agree, your phone keeps sealed messages for other people in memory for up to 24 hours and passes them on or uploads them. It cannot open them, and they are not saved to storage. Limits on size, count and how often a phone can send stop it being used to flood you.

### Crash and fall detection

Crash and fall detection is off until you turn it on. When it is on, the app reads your phone's motion sensors while it watches, looking for a hard knock followed by stillness. The readings stay in memory for a few seconds and are then dropped. They are never saved or sent. If the app thinks there was a crash or fall and you do not answer the 30 second countdown, it sends an alert to your chosen people the usual way, with your location if you allowed it.

It is not a certified safety or medical device. It can miss a real crash or fall, and it can go off when nothing is wrong.

### Your watch

If you turn on the watch trigger, holding SOS on your watch sends a short "start" message to your phone. On Apple Watch this goes over Apple's WatchConnectivity link between your watch and your phone. On Wear OS it goes through Google Play services on your phone and watch, which can pass it through Google's network when the two are not connected directly. The message holds no location, people or details. The phone then shows its usual countdown and sends the alert itself.

### Live streams, uploads and recordings

If you turn on live streaming or uploads, your video and sound go to the service or server you set up, such as YouTube, Twitch or your own server. You sign in to that service yourself. If you share a recording, it goes wherever you send it. Those services have their own privacy policies. Please read them before you use them.

**Live backup.** If you turn on live backup for an emergency type (off by default), each part of a recording is uploaded while it records, only to the WebDAV or S3 storage you set up yourself, with the signed list of fingerprints. Nothing goes to Upton Software Ltd. Liability Company. By default the copies stay encrypted, so the storage provider cannot watch them. To let you open them without your phone, the app also uploads a key file locked with a backup passphrase you choose (Argon2id and AES-256-GCM). The app never stores or uploads the passphrase itself, and the company cannot recover it. If you choose "readable copies" instead, plain unencrypted copies go to your storage, and anyone who can get into it can watch them. The readable copy of each part is made on your phone just before it is uploaded and deleted right after (and at the next launch, if the app was closed mid-upload). Uploads that have not finished wait in an encrypted list on your phone and carry on when the app next runs. If you end an alert with your duress PIN, parts already recorded keep uploading quietly.

Cameras, Bluetooth devices and network devices you connect get only the commands needed to start and stop recording.

### Exports

If you export a recording, the app makes plain, unencrypted copies of it, with a manifest.json and a verification.txt, and opens your device's share sheet. The manifest lists when and where each part was recorded, the recording device, and your public key, its fingerprint and your app code. If you export your alert history, the app makes a report (HTML), a CSV and a JSON file with everything in the history. These files are not encrypted. They go only where you send them. The app makes them in its own private folder and deletes them, and the copies the share sheet makes, once the share sheet closes; anything left over (for example if the app was closed while sharing) is deleted the next time the app opens and when an alert ends. Share them only with people you trust.

"Make a file for a lawyer" puts one alert's recordings, signed notes, location trail, delivery log and signatures into a single file locked with a passphrase you choose (Argon2id and AES-256-GCM). The app never uploads it. It opens your share sheet and you choose where it goes. Anyone with the file and the passphrase can see everything in it, so give the passphrase separately.

### Backups

If you save a backup, the app makes a file locked with a passphrase you choose. It can include your alert history if you leave that on. It never includes recordings. You decide where the file goes. If you keep it in a cloud service, that service's policy applies. Upton Software Ltd. Liability Company cannot open your backup and cannot recover a lost passphrase.

## Your responsibility for other people's data

The people you add, and anyone you record, have their own privacy rights. Add only people who agree to get your alerts. If you record or stream other people, check the law where you are first. This also applies to sound recordings without an alert, to dashcam mode, and to letting someone listen through an answered call. Keeping this data on your own phone for personal use is usually outside data protection law, but sharing recordings publicly may not be.

## Permissions and why the app asks

The app asks for each permission only when you use the feature that needs it. You can say no and still use the rest of the app.

- Location: to add where you are to an alert. It is read while an alert is running, while a check-in timer is running (so the alert can carry your last known location if you do not check in, and a trip can say where you are), once when a low battery alert is sent, and, as its last known location, when the traffic stop rights card is shown (to pick the area on your device, not saved or sent), when you save a note, and when you start a sound recording without an alert (kept with the note or recording on your device). It is also read when a person you allowed asks where you are, and then sent only to that person. On Android, if you leave the app during an alert, location updates carry on until you end the alert, and a notification shows while they do. It is not read at any other time.
- Notifications: to remind you before a check-in timer runs out (5 minutes and 1 minute before, and when it is due), and to tell you when a person asked your phone for your location or a recording. On Android they are also used for the recording, sound recording, dashcam, volume button and crash or fall detection notices, and to offer dashcam mode when your car connects. Reminders are made on your device. They do not go through Upton Software Ltd. Liability Company or any server.
- Alarms and reminders (Android): so a check-in timer goes off on time, even if the app is closed or the phone restarted. Without it, Android may run the timer late.
- Camera: to scan a person's QR code, to record or stream video during an alert if you turn that on, and for dashcam mode with video.
- Microphone: to record sound during an alert if you turn that on, when you start "Record sound only", and for dashcam mode. If you leave the app while it records, sound keeps recording until you stop it (or end the alert). On Android, phone video keeps recording too. On iPhone and iPad, phone video switches to sound only while the app is out of view, because iOS does not allow it.
- Bluetooth (on Android, "Nearby devices"): to start a camera or trigger button when you send an alert, if you turn on nearby delivery, to pass your encrypted alert to phones close by, and, for "Start dashcam in my car", to list the phone's paired devices and notice when your car connects. It does not scan for that.
- Phone, Contacts and caller ID and spam app (Android only): for "Answer calls during an alert", if you turn it on. See "Answering calls during an alert" above.
- Volume buttons: no permission. On Android, while you have armed the volume button trigger, a notification shows that it is ready. On iPhone and iPad it works only while the app is open on screen.
- Motion sensors: for crash and fall detection, if you turn it on. On Android, while detection is on and the app is closed, a notification shows that it is watching.
- Local network: to reach cameras, triggers and servers you set up on your own network.
- Photos (save only): to save recordings to your photo library when you ask.
- Internet: to send encrypted app messages through relays, and for streams and uploads you set up.

## Things Upton Software Ltd. Liability Company does not do

- The company does not sell or share your personal information, as "sell" and "share" are defined in California law. It has none to sell.
- The company does not track you across apps or websites, and no one else can through its app.
- The company does not use advertising, analytics or tracking tools.
- The company does not build profiles or make automated decisions about you.

## Users in the United States

Upton Software Ltd. Liability Company collects nothing through the app, sells nothing and shares nothing. It does not sell or share personal information, or use it for targeted advertising, as state privacy laws such as the California Consumer Privacy Act (as amended by the CPRA) define those terms. It does not use sensitive personal information. If you email the company, it uses your email only to answer you. If your state gives you rights over personal data, such as the right to know, correct or delete it, you can use them by emailing the company. The company will not treat you differently for doing so.

## Do Not Track

The app collects nothing about your activity, on its own or across other apps and websites. So it does not respond differently to Do Not Track or Global Privacy Control signals. There is nothing to switch off.

## Children

Project S.O.S is a general app. It is not meant for children under 13, and it is not aimed at children. Upton Software Ltd. Liability Company does not knowingly collect personal data from anyone, of any age, and the app sends the company nothing. That includes children under 13, as the US Children's Online Privacy Protection Act (COPPA) defines them. If you think a child under 13 has emailed the company, tell it and it will delete the email. If a parent or guardian sets the app up for a child, the child's data stays on the child's device and goes only to the people the parent or child chose.

## Deleting your data

You can delete people, groups and emergency types in the app at any time. In Settings, Data, Alert history you can delete one alert, or all of them, with their recordings. Notes written without an alert can be deleted in History.

To delete everything at once, go to Settings, then Data, then Delete my profile. If an alert or a check-in timer is running, end it first. Read what will be deleted, then hold the button until it fills (or tap to delete instead, and confirm). The app deletes, from your device, your username and your identity keys in the Keychain or Keystore, your people, groups and emergency types, recordings and their keys, history and notes, trips, check-in timers, settings, saved and cached files, and scheduled reminders and alarms. It then starts again as if newly installed. This cannot be undone. People who added you keep your old app code until they remove you. The steps are also at https://elderguardadmin-byte.github.io/project_s.o.s_privacy_policy/delete-your-data.

Upton Software Ltd. Liability Company holds none of this data, so there is nothing for the company to delete on its side. Panic wipe (above) also makes everything on the device unreadable. Uninstalling the app removes everything it stored on your device. Backups you saved elsewhere are yours to delete. Messages already delivered stay on the recipient's phone, and a relay may keep its copy of an encrypted message for a while. Streams and uploads stay with the service you sent them to, under your account there.

To have your support emails deleted, email Upton Software Ltd. Liability Company.

## Your rights

Depending on where you live, you may have rights over personal data that Upton Software Ltd. Liability Company holds. These can include the right to see it, correct it, delete it, object to how the company uses it, or get a copy. This applies in the UK, the EU and EEA, California and other US states, Canada, Australia and elsewhere. Because the company holds only support emails and store reports, there is usually little for it to provide. You can still ask. The company will reply within one month. It will not treat you differently for using your rights.

Data on your device is in your control. Use the app to see, change or delete it.

Upton Software Ltd. Liability Company has not named a representative in the UK or the EU. The law does not require one when a company's processing is occasional and low risk. The company's only processing is answering the support emails people choose to send. To use your rights, contact the company directly at the email below.

If you are unhappy with how Upton Software Ltd. Liability Company handled your data, please tell the company first. You can also complain to a data protection authority. In the UK that is the Information Commissioner's Office (ico.org.uk). In the EU and EEA, it is the authority in your country. In Canada it is the Office of the Privacy Commissioner, and in Australia the Office of the Australian Information Commissioner.

## Changes to this policy

If Upton Software Ltd. Liability Company changes this policy, the company will update it in the app and at https://elderguardadmin-byte.github.io/project_s.o.s_privacy_policy/, with a new effective date. If a change affects how your data is handled, the company will also say so in the release notes for that version of the app.

## Contact

Upton Software Ltd. Liability Company
Email: elderguardadmin@elderguard.info
Phone: +1 770-275-1992
Post: 8735 Dunwoody Place, Atlanta, GA 30350, USA
