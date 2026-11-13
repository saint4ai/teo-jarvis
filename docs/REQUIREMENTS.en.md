# System requirements

[Русская версия](REQUIREMENTS.md) · [Back to README](../README.en.md)

Two levels. **Minimum:** Teo runs in a light mode, and some features are simpler. **Recommended:** everything is on.

## Windows

| | Minimum | Recommended |
|---|---|---|
| OS | Windows 10 (1809 or newer) or Windows 11, 64-bit | Windows 11 or Windows 10 22H2, 64-bit |
| CPU | 4 threads with the AVX2 instruction set. As a guide: Intel Core 8th generation or newer, AMD Ryzen | 4 cores and 8 threads (Core i5 8th generation or newer, Ryzen 5) |
| RAM | 8 GB | 16 GB |
| Disk | 3 GB free | 5 GB free on an SSD |
| Microphone | any working one | a headset if the room is noisy |
| Internet | constant access to Claude | a stable connection |
| GPU | any with DirectX 11 | integrated Intel UHD 620 or newer, or a separate graphics card |

Intel Celeron and Pentium models from 2018 and 2020 are below the minimum: they do not have AVX2.

## macOS

| | Minimum | Recommended |
|---|---|---|
| OS | macOS 13 or newer | macOS 15 or newer |
| CPU | Apple M1 or newer. Macs with Intel processors are not supported | Apple M1 or newer |
| RAM | 8 GB | 8 GB |
| Disk | 3 GB free | 5 GB free |
| Microphone | the built-in one works | a headset in a noisy room |

macOS asks for permissions one at a time, when Teo first needs each one: Microphone (required), Accessibility (for the Teo key, windows and typing text), Screen Recording, Automation and Notifications (optional).

## Also needed

- A Claude Pro or higher subscription, or your own Anthropic API key.
- For Kazakh and the cloud voice: your own ElevenLabs API key (optional).
- You do not need to install anything first: no Python, no Node.

## How Teo checks your computer

On first launch, and when you press "Re-measure computer" («Перемерить компьютер») in Settings: up to 10 seconds, with no sound and no windows. Teo names one of three levels: recommended, minimum or below minimum. The beta does not start on a computer below the minimum, and Teo tells you why.
