# What Teo does with your data

[Русская версия](PRIVACY.md) · [Back to README](../README.en.md)

This is a short summary. The full privacy policy is on the Teo server: [teo.onai.academy/privacy](https://teo.onai.academy/privacy), in Russian and Kazakh.

Teo lives on your computer. Memory, chats, logs and keys stay with you. Only what is needed for an answer leaves the computer.

## What stays on your computer

- Teo's memory: what you asked it to remember, and your profile from "Getting to know you".
- The log of Teo's actions and notes about failures.
- The Telegram and WhatsApp chats you connected, with their voice messages. WhatsApp arrives through the Teo server but is not stored there (see below).
- Service keys, in Windows Credential Manager or in the macOS Keychain.
- The sign-in to Claude happens in the Claude app itself. Teo does not see or store your subscription key.
- Speech recognition and the "Male 5" voice («Мужской 5») run on your computer.

You can set a retention period, and older data is then erased automatically. Without a period, Teo deletes nothing.

## What leaves your computer

| Where to | What | When | How to turn it off |
|---|---|---|---|
| Claude (Anthropic) | What you said. Parts of files, emails, web pages and messages you asked Teo to look at. A screenshot of the window when you use "Explain screen" («Объяснить экран») | With every answer | Not completely: Teo works through Claude. You can leave mail and chats unconnected and not ask Teo to read files or the screen |
| ElevenLabs | The answer text, to turn it into speech. Your speech audio when you dictate in Kazakh | Only if you chose the cloud voice or Kazakh and entered your own key | Choose "On-device voice" («Голос на компьютере») or "Text only" («Только текст») |
| Hugging Face | Nothing of yours. Teo downloads models | Once, on first launch | Not possible without losing speech recognition |
| GitHub | Nothing of yours. Once a day Teo requests the version description and downloads the update | 10 minutes after launch, then once a day | Turn it off in the update settings |
| Teo account server | Your Telegram account number, subscription and trial dates, Teo version, the number of requests per day without their text. Fingerprints of your phone and computer, not the values themselves. If you sign in with email and password: your email address in encrypted form, the password only as a hash, and your country from a list. We do not send emails to that address yet | At sign-in and once a day | Delete your account on the account page |
| Teo server (WhatsApp) | New WhatsApp messages pass through the server to your computer. The server keeps them in memory until Teo picks them up, for no longer than 72 hours, and never writes them to disk. Files are streamed. WhatsApp contacts (number, name, profile photo) stay on the server while WhatsApp is connected | Only if you connected WhatsApp | Log out of WhatsApp in Connections: the session and contacts are deleted at once |
| Developer server | Teo errors and crashes, without conversations, files or keys | Automatically, in the beta | The switch in Settings, the "Privacy" block («Приватность») |
| Developer server | A support report and feedback | Only when you press the button | Do not press it |

## What Teo does not do

- Does not store chats on the developer server. WhatsApp only passes through the Teo server.
- Does not store keys in plain text and does not pass them to the app window.
- Does not run text from chats, mail, websites or files as a command.
- Does not delete or clean up files and does not install apps without your "yes". A message goes out after 5 seconds, and you can cancel it in that time.
