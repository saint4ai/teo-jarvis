# Teo FAQ

[Русская версия](FAQ.md) · [Back to README](../README.en.md)

## About Teo

### What is Teo and how is it different from Claude?

Teo is a voice assistant for your computer, in the spirit of Jarvis. Claude runs inside, but you never touch its interface. You speak or type to Teo, and it opens apps, finds files, reads mail and gets things done.

### Do I need a Claude subscription?

Yes. Teo thinks and answers through Claude, so you need Claude Pro or higher (about $20 a month on the Anthropic site), or your own Anthropic API key. Teo guides you through the sign-in in the setup wizard.

### Do I need Python, Node or a terminal?

No. Everything is inside the installer or downloads on first launch.

### How much does Teo cost?

The beta is free for 14 days with every feature. No card needed.

### Which languages work?

The interface and answers are in Russian. Speech recognition covers Russian and English. Kazakh works through ElevenLabs with your own key.

### Why "Jarvis"?

People call voice assistants that do things for you "Jarvis". Teo is such an assistant. It has no connection to any company or character with that name.

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

The sums must match character for character. If they do not, do not run the file and open an [issue](https://github.com/saint4ai/teo-jarvis/issues/new/choose).

### How much do I download?

The installer is about 300 MB. On first launch Teo downloads about 770 MB more: speech recognition (about 640 MB) and the memory model (about 130 MB). The on-device voice adds about 123 MB.

| Internet speed | Model download time |
|---|---|
| 5 Mbit/s | about 21 minutes |
| 20 Mbit/s | about 5 minutes |
| 100 Mbit/s | about 1 minute |

You can go through the wizard steps while the files download.

### Will my computer run Teo?

See the [requirements](REQUIREMENTS.md). On first setup Teo measures your computer (about 15 seconds, silent) and names a level. Between minimum and recommended, Teo switches to a light mode and tells you what is turned off. Below minimum, Teo says so honestly and the trial does not start.

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

1. Check the microphone in the wizard step "Microphone" or in Settings.
2. Windows: Settings, Privacy, Microphone. Turn on "Let desktop apps access your microphone".
3. macOS: System Settings, Privacy and Security, Microphone. Turn Teo on.
4. A headset works better in a noisy room.
5. Instead of the word you can press the Teo key (Pause on Windows, right Option on Mac) or type the task.

### How do I stop Teo?

Press the Teo key again or click "Stop" in the capsule. While the microphone is open, the words "stop" and "enough" work too.

### Teo answers itself

While Teo speaks or plays a sound, the microphone is deaf. If Teo still took its own answer for a command, press "Leave feedback" and tell us the app and the voice you used.

### How do I connect Gmail and Google Drive?

Through Claude. Four steps: [CONNECTORS.md](CONNECTORS.md).

### What is the Teo browser?

A separate browser with its own profile. Sign in to the services you need and the sign-ins stay on this computer only. Teo can do anything you ask in it on your behalf. Teo warns you before the first launch.

### Teo got it wrong. How do I fix that?

Say "Teo, remember that ..." and explain the right way. For disputed cases Teo keeps a log: control panel, Home, block "What Teo did and where it stumbled".

## Data and safety

### Where does my data go?

In short: memory, chats, logs and keys stay on your computer. To answer, Claude receives what you said and the parts of files, mail and pages you asked Teo to open. Full table: [PRIVACY.md](PRIVACY.md).

### Can Teo send or delete something without asking?

No. Sending messages, closing apps, cleanup and other risky actions go through a "Yes" or "No" card. Teo does not run text from chats, mail and websites as a command.

## Bugs and feedback

### How do I report a bug?

Any of these:

- Say "Teo, log a bug".
- Press "Support report" in Settings. The report is built and sent only when you press the button. It holds no keys and no chats.
- Press "Leave feedback" in the same place.
- Open an [issue](https://github.com/saint4ai/teo-jarvis/issues/new/choose). Do not attach keys, passwords or private chats.

### What does Teo send to the developers by itself?

In the beta Teo sends errors and crashes without the text of your conversations, files or keys. The switch is in Settings, block "Privacy".
