<p align="center">
  <img src="assets/hero.png" alt="Teo: a Jarvis-style voice AI assistant for Windows and macOS. Listening capsule and a five-button control panel" width="100%">
</p>

# Teo: a Jarvis-style voice AI assistant for your computer

**Jarvis for your own computer.** Say "Teo" and it opens apps, finds files, reads your mail or edits a spreadsheet. It runs on Claude. Windows and macOS.

Beta 1.0.0-beta.1: **14 days free, every feature included. Then $10 a month.**

![Status](https://img.shields.io/badge/status-beta-e8c887?style=flat-square)
![Windows](https://img.shields.io/badge/Windows-10%20and%2011-3b82f6?style=flat-square&logo=windows&logoColor=white)
![macOS](https://img.shields.io/badge/macOS-13%2B%20%28Apple%20Silicon%29-555?style=flat-square&logo=apple&logoColor=white)
![Price](https://img.shields.io/badge/beta-14%20days%20free%2C%20then%20%2410%20a%20month-2ea043?style=flat-square)
![Runs on Claude](https://img.shields.io/badge/runs%20on-Claude-d97757?style=flat-square)

**[Download the beta](https://github.com/saint4ai/teo-jarvis/releases)** · [Install](#install) · [Features](#what-teo-does) · [FAQ](docs/FAQ.en.md) · [Русский](README.md)

---

## What is Teo

Teo is a voice assistant that lives on your computer. It hears the wake word "Teo", understands speech and does the work inside your apps. The interface is in Russian today. English speech recognition works too.

Claude runs inside, through your own Claude subscription. You do not need a terminal, config files or permission prompts. Install Teo, sign in to Claude and talk.

- A capsule at the top of the screen shows when Teo listens, thinks or answers.
- A control panel with five buttons keeps everything in one place: Home, Tasks, Skills, Connections, Settings.
- Teo comes as a normal installer. No Python, Node or other tools to set up first.

![Teo capsule: listening, working, speaking, asking before a risky action and showing agents](assets/screens/capsule-states.png)

## What Teo does

| Area | Example phrase |
|---|---|
| **Apps and windows.** Open, close, snap to a side, lower the volume | "Open Telegram", "Snap Chrome to the left" |
| **Files and documents.** Find a file, read it, edit Word and Excel, make a PDF | "Find the file contract", "Make an Excel sheet of monthly expenses" |
| **Mail and calendar.** Gmail, Yandex and Mail.ru with an app password. Calendar by link | "What important mail came in", "Reply to the last client email" |
| **Google Drive and other services** through Claude connectors | "Find the contract on Drive" |
| **WhatsApp and Telegram.** Sign in with a QR code or a phone number. Teo reads chats and replies after your "yes" | "Who is waiting for a reply", "Write to Marina: I will be there in an hour" |
| **Voice messages.** Teo transcribes them and gives you the short version | "What is in Marina's voice message" |
| **Web video.** Pause, next episode, full screen on YouTube and other sites | "Pause the video", "Full screen" |
| **Memory and reminders.** Teo remembers who you are and where things live | "Remember that reports should be short", "Remind me at six to send the invoice" |
| **Claude Code agents.** See who is working, who waits for you, who is done. Approve agent requests from the capsule | "Which agents are waiting for me" |
| **Skills.** Ready-made abilities, plus new ones Teo writes for itself | "What skills do you have" |
| **Dictation into any window.** Hold a key, speak, the text lands where your cursor is | Shift and the Teo key |

Before a risky action Teo shows a card and waits for "yes" or "no". Sending messages, closing apps and cleanup happen only after you agree.

### Voice

- **"Мужской 5" (Male 5)**, the on-device voice: free, works offline. Teo downloads it on first launch.
- **ElevenLabs**: a lively cloud voice with your own key. Also needed for Kazakh.
- **Text only**: answers appear on screen, no sound.

Speech recognition runs on your computer. Languages: Russian and English. Kazakh goes through ElevenLabs with your key.

## Screenshots

All screenshots use demo data. Names, emails and numbers are made up.

| Home | Tasks |
|---|---|
| ![Home screen of the Teo control panel](assets/screens/home.png) | ![Tasks screen of the Teo control panel](assets/screens/work.png) |

| Skills | Connections |
|---|---|
| ![Skills screen of the Teo control panel](assets/screens/skills.png) | ![Connections screen of the Teo control panel](assets/screens/connections.png) |

![Settings screen of the Teo control panel](assets/screens/settings.png)

## Install

### Requirements

- Windows 10 (version 1809 or newer) or 11, 64-bit. Or macOS 13 or newer on an Apple M1 chip or newer.
- A Claude Pro subscription or higher (about $20 a month on the Anthropic site). Or your own Anthropic API key.
- 8 GB of RAM and 3 GB of disk space. 16 GB and 5 GB on an SSD is better.
- A microphone and an internet connection.
- A Telegram account: you sign in to Teo with it.

Details: [docs/REQUIREMENTS.md](docs/REQUIREMENTS.md).

### Windows

**1.** Open [Releases](https://github.com/saint4ai/teo-jarvis/releases) and download `Teo-Setup-1.0.0-beta.1.exe`. The browser may ask about the file: click Keep.

**2.** Run the file with a double click. No administrator rights needed.

<img src="assets/install/windows-1-more-info.png" alt="Windows window: click More info" width="560">

**3.** Windows warns about an unknown publisher. Click "More info".

<img src="assets/install/windows-2-run-anyway.png" alt="Windows window: click Run anyway" width="560">

**4.** Click "Run anyway".

**5.** Wait for the install to finish. Teo opens and walks you through setup. It takes about 5 minutes.

The windows in the pictures are a drawn scheme of the real Windows windows. The window appears because the installer has no paid code signing certificate yet. The file is the same. You can verify it with the SHA-256 sum in the release notes: [how to verify](docs/FAQ.en.md#how-do-i-verify-the-file). The file will not open? [FAQ](docs/FAQ.en.md#installing).

### macOS

The Mac image is added to the release separately from the Windows installer. If there is no `.dmg` file in the release yet, the Mac version is being prepared.

![Teo disk image: drag Teo to Applications](assets/install/mac-1-dmg.png)

**1.** Download the `.dmg` file from [Releases](https://github.com/saint4ai/teo-jarvis/releases), open it and drag Teo to Applications.

<img src="assets/install/mac-2-dialog.png" alt="macOS warning: click Done" width="320">

**2.** Launch Teo. macOS warns that the app is not verified. Click "Done" (the button in Russian macOS is «Готово»). Do not click the button that moves Teo to the Bin: it removes Teo.

![Security settings: click Open Anyway](assets/install/mac-3-open-anyway.png)

**3.** Open System Settings, Privacy and Security. Scroll down to Security and click "Open Anyway".

**4.** Enter your Mac password or use Touch ID. You do this once.

The pictures show the name "Тео Проба": that is a trial app with the same signature. You will see "Тео". A window says the app is "damaged"? Click OK, Teo is running. Did not help? [Detailed guide](docs/INSTALL-MAC.en.md).

After launch macOS asks for microphone and other permissions one by one, when Teo first needs them.

### First launch

A setup wizard walks you through: computer check, Teo account, microphone, wake word, Claude sign-in, voice, first command.

**Teo account.** Click "Create account" (in the app: «Создать аккаунт»). Teo opens a sign-in page in your browser.

1. Match the code on the page with the code in the Teo window.
2. Tick both boxes: terms and offer, data processing. Click "Continue".
3. Confirm the sign-in through Telegram. The sign-in bot is @teojarvis_bot.

No password. The 14-day trial starts with your first sign-in.

On first launch Teo downloads two models: speech recognition (about 640 MB) and memory (about 130 MB). That is about 5 minutes at 20 Mbit/s. You can go through the steps while they download.

> The wizard screenshots use demo data. In the beta there is one more step, "Teo account", between the greeting and the microphone.

### Connect Google Drive, mail and calendar

Google Drive and other services connect through Claude. Mail and calendar are set up separately. Guide: [docs/CONNECTORS.md](docs/CONNECTORS.md).

## Beta: 14 days free, then $10 a month

| | |
|---|---|
| **Trial** | 14 days, every feature. No card asked. It starts with your first sign-in |
| **After that** | $10 a month, one plan. The amount in the payment currency is shown on the payment page before you pay. No auto-renewal: you renew yourself |
| **Where to pay** | In Teo: Settings, "Teo account and subscription" |
| **Two ways** | "Payment Russia" («Оплата Россия»): a card from a Russian bank, paid at once. "Payment other countries" («Оплата другие страны»): a card from a bank outside Russia, the payment link arrives by SMS |
| **Refund** | We refund the days that have not started yet. Terms in the [offer](https://teo.onai.academy/terms) |
| **After 14 days without payment** | AI answers switch off. Commands without AI, memory and settings stay |
| **Computer** | One account, one computer. You can move it once in 30 days |

You can see your account, subscription and payments on the [teo.onai.academy/account](https://teo.onai.academy/account) page. You can also unlink the computer or delete the account there.

## Support

- Email: [saint4aiinst@gmail.com](mailto:saint4aiinst@gmail.com). Give your account number: it is on the account page.
- The "Leave feedback" form in Teo: Settings, Support block. Send ideas there too.
- Teo sends error reports to the developers by itself, without your conversations, files or keys. You can turn this off in Settings, Privacy block.

## Privacy

Memory, logs, chats and keys stay on your computer. To answer, Claude receives what you said and the parts of files, mail and pages you asked Teo to open. The cloud voice runs only with your own key.

Details: [docs/PRIVACY.md](docs/PRIVACY.md). The full policy on the Teo server: [teo.onai.academy/privacy](https://teo.onai.academy/privacy).

## Teo and other Jarvis projects

Most Jarvis projects on GitHub need to be built from source: Python, API keys, a terminal. Teo installs with an installer and guides you through setup.

Teo started as a fork of the open-source [JARVIS](https://github.com/adewaskar/jarvis) project by Aditya Dewaskar (MIT). Thank you to the author. See [NOTICE.md](NOTICE.md).

## Roadmap and docs

[Roadmap](docs/ROADMAP.md) (directions, no dates) · [Changelog](CHANGELOG.md) · [FAQ](docs/FAQ.en.md) · [Mac install](docs/INSTALL-MAC.en.md) · [Requirements](docs/REQUIREMENTS.md) · [Privacy](docs/PRIVACY.md) · [Offer](https://teo.onai.academy/terms) (Russian and Kazakh) · [Security](SECURITY.md) · [License](LICENSE)

---

*Teo runs on Claude. Claude is a trademark of Anthropic. Teo is not affiliated with Anthropic. "Jarvis" here names a type of assistant, not a product or a character of any company. This repository holds installers and release notes. There is no Teo source code here.*
