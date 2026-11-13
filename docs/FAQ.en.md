# Teo FAQ

[Русская версия](FAQ.md) · [Back to README](../README.en.md)

## About Teo

### What is Teo and how is it different from Claude?

Teo is a voice assistant for your computer, in the spirit of Jarvis. Claude runs inside, but you never touch its interface. You speak or type to Teo, and it opens apps, finds files, reads mail and gets things done.

### Do I need a Claude subscription?

Yes. Teo thinks and answers through Claude, so you need Claude Pro or higher (from $20 a month on the Anthropic site), or your own Anthropic API key. Teo setup guides you through the sign-in. Claude is not available in every country: check that it opens for you before you pay.

### Do I need Python, Node or a terminal?

No. Everything is inside the installer or downloads on first launch.

### How much does Teo cost?

The first 14 days are free with every feature. No card needed. After that it is $10 a month, one plan. The amount in the payment currency is shown on the payment page before you pay. No automatic charges: you renew yourself. More: [Account and payment](#account-and-payment).

### Which languages work?

The interface and answers are in Russian. Speech recognition covers Russian and English. Kazakh works through ElevenLabs with your own key.

### Why "Jarvis"?

People call voice assistants that do things for you "Jarvis". Teo is such an assistant. It has no connection to any company or character with that name.

## Account and payment

### How do I sign in to Teo?

Two ways: with email and password, or with Telegram. In Teo setup click "Create account" («Создать аккаунт») or "Sign in" («Войти»). A sign-in page opens: match the code with the code in the Teo window and tick both boxes.

- **With email.** Enter your email, a password of at least 8 characters, the password again, and choose your country: the payment currency depends on it. We do not send emails yet, and the email address is not verified.
- **With Telegram.** Click the Telegram button. Telegram sends you the message "We received a request to log in". Tap "Accept" in it. The sign-in bot is @teojarvis_bot.

You can add the second sign-in method later on the [teo.onai.academy/account](https://teo.onai.academy/account) page.

Forgot your password? If a Telegram account is linked, sign in with it on the account page and change the password. If not, write to [saint4aiinst@gmail.com](mailto:saint4aiinst@gmail.com).

### What happens after 14 days?

AI answers switch off until you pay for the subscription. Commands without AI, memory and settings stay. Teo shows a screen with the payment buttons.

### How do I pay?

In Teo: Settings, "Teo account and subscription". Two ways:

- "Pay with a Russian bank card" («Оплата Россия»): a card from a Russian bank, paid at once on the page.
- "Pay with a card from another country" («Оплата другие страны»): a card from a bank outside Russia, the payment link arrives by SMS.

You enter the card details only on the payment page. Teo never receives them. The amount in the payment currency is shown before you pay. There are no automatic charges: you renew yourself.

### Can I get a refund?

Yes. Write to [saint4aiinst@gmail.com](mailto:saint4aiinst@gmail.com) or press "Send feedback" («Оставить отзыв») in Teo. We refund the days that have not started yet. If Anthropic blocked your Claude account, we refund the last payment if less than 30 days have passed. All terms are in the [offer](https://teo.onai.academy/terms) (Russian and Kazakh).

### Can I use Teo on two computers?

One account works on one computer. You can move it once in 30 days. On the [teo.onai.academy/account](https://teo.onai.academy/account) page you can unlink a computer.

### Is the trial given a second time?

No. The trial is given once per email, once per Telegram account and once per computer.

### How do I delete my account?

On the [teo.onai.academy/account](https://teo.onai.academy/account) page. Deleting closes the subscription. On your request we refund the days that have not started yet.

## Installing

### Windows says "Windows protected your PC". What do I click?

Click "More info", then "Run anyway". Every installer without a paid code signing certificate triggers this window. Teo does not have one yet.

No window, but the file will not open? Right-click the file, choose Properties, tick "Unblock" and click OK.

### The browser says the file is rarely downloaded

That is a browser warning, not a Windows one. Click Keep.

### macOS will not open Teo

The app has no Apple signature yet. Open System Settings, Privacy and Security, scroll down and click "Open Anyway". Enter your Mac password. You do this once.

### How do I verify the file?

Easy way: right-click the file and choose "Scan with Microsoft Defender".

Careful way: every installer has a SHA-256 sum in the release notes. Compute it yourself and compare.

Windows PowerShell:

```
Get-FileHash .\Teo-Setup-<version>.exe -Algorithm SHA256
```

macOS:

```
shasum -a 256 <file>.dmg
```

The sums must match character for character. If they do not, do not run the file and write to [saint4aiinst@gmail.com](mailto:saint4aiinst@gmail.com).

### How much do I download?

The installer is about 300 MB. On first launch Teo downloads about 770 MB more: speech recognition (about 640 MB) and the memory model (about 130 MB). The on-device voice adds about 123 MB.

| Internet speed | Model download time |
|---|---|
| 5 Mbit/s | about 21 minutes |
| 20 Mbit/s | about 5 minutes |
| 100 Mbit/s | about 1 minute |

You can go through the setup steps while the files download.

### Will my computer run Teo?

See the [requirements](REQUIREMENTS.en.md). On first setup Teo measures your computer (up to 10 seconds, silent) and names a level. Between minimum and recommended, Teo switches to a light mode and tells you what is turned off. Below minimum, Teo says so honestly and the trial does not start.

### How do I update Teo?

A new version appears as a card on Home. Click "Update" («Обновить»): Teo downloads it and restarts by itself, in about a minute. On Mac the "Download" button («Скачать») opens the release page: install the new version over the old one, as you did the first time.

### How do I uninstall Teo?

Windows: Settings, Apps, find Teo and click Uninstall. Teo asks whether to erase memory, settings and models.

Remove the keys in Credential Manager (`Teo/...`) and the `Documents\Тео` folder yourself.

Answered "no" and now want everything gone? Delete these folders:

- `%APPDATA%\Тео`
- `%LOCALAPPDATA%\Teo`
- `C:\ProgramData\Teo`, if your Windows profile name has Cyrillic letters

macOS: drag Teo from Applications to the Trash. Data lives in `~/Library/Application Support`, in the Teo folder.

## Using Teo

### Teo does not hear the wake word

1. Check the microphone in the "Microphone" setup step or in Settings.
2. Windows: Settings, Privacy, Microphone. Turn on "Let desktop apps access your microphone".
3. macOS: System Settings, Privacy and Security, Microphone. Turn Teo on.
4. A headset works better in a noisy room.
5. Instead of the word you can press the Teo key (Pause on Windows, right Option on Mac) or type the task.

### How do I stop Teo?

Press the Teo key again or click "Stop" in the capsule. While the microphone is open, the words "stop" and "enough" work too.

### How do I quit Teo completely?

Click "Quit Teo" («Выйти из Тео») at the top of the Dashboard or in the menu of the Teo icon next to the clock. Teo asks «Тео перестанет слушать. Выйти?» ("Teo will stop listening. Quit?"). Click "Quit" («Выйти»).

### Teo answers itself

While Teo speaks or plays a sound, the microphone is deaf. If Teo still took its own answer for a command, press "Send feedback" and tell us the app and the voice you used.

### How do I connect Google Drive, mail and calendar?

Google Drive, Google Calendar and other services connect through Claude connectors, four steps. Mail is set up in Teo separately, with an app password. All in [CONNECTORS.en.md](CONNECTORS.en.md).

### What is the Teo browser?

A separate browser with its own profile. Sign in to the services you need and the sign-ins stay on this computer only. Teo can do anything you ask in it on your behalf. Teo warns you before the first launch.

You choose which browser Teo works in under Connections, on the "Teo browser" card («Браузер Тео»). By default it is the main browser of your system. Chrome, Edge and Yandex Browser work.

### Teo got it wrong. How do I fix that?

Say "Teo, remember that ..." and explain the right way. For disputed cases Teo keeps a log: Dashboard, Home, the "What Teo did and where it got stuck" block («Что Тео сделал и где споткнулся»).

## Data and safety

### Where does my data go?

In short: memory, chats, logs and keys stay on your computer. To answer, Claude receives what you said and the parts of files, mail and pages you asked Teo to open. Full table: [PRIVACY.en.md](PRIVACY.en.md). The full policy on the Teo server: [teo.onai.academy/privacy](https://teo.onai.academy/privacy).

### Can Teo send or delete something without asking?

It cannot delete without your "yes": deleting, cleanup and installing apps go only through a confirmation card with "Yes" and "No". Teo does a clear request right away. A message goes out after 5 seconds, and you can cancel it in that time. If the recipient is unclear, or Teo read someone else's text for this task, it asks with a card first. Teo does not run text from chats, mail and websites as a command.

## Bugs and feedback

### How do I report a bug?

Any of these:

- Say "Teo, log a bug".
- Press "Support report" in Settings. The report is built and sent only when you press the button. It holds no keys and no chats.
- Press "Send feedback" in the same place.
- Write to [saint4aiinst@gmail.com](mailto:saint4aiinst@gmail.com) and give your account number: it is on the [teo.onai.academy/account](https://teo.onai.academy/account) page. Do not attach keys, passwords or private chats.

### What does Teo send to the developers by itself?

In the beta Teo sends errors and crashes without the text of your conversations, files or keys. The switch is in Settings, block "Privacy".
