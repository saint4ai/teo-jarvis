# Security

[Русская версия](SECURITY.md) · [Back to README](README.en.md)

## Reporting a vulnerability

Found a vulnerability in Teo? Do not open a public issue.

1. Open the **Security** tab of this repository and click **Report a vulnerability**. Only the developers see your report. If that does not work, write to [saint4aiinst@gmail.com](mailto:saint4aiinst@gmail.com) with the subject "Vulnerability".
2. Describe what you found, how to reproduce it and what could happen.
3. Do not attach keys, passwords or other people's personal data.

## What we care about most

- Text from outside (chats, mail, websites, files) must not control Teo (prompt injection).
- Deleting, cleanup and installing apps happen only after the person says "yes". A message goes out after 5 seconds, and the person can cancel it in that time. Teo closes an app without asking only when the person named that app. Teo does not press payment buttons.
- Keys and sign-ins must not reach the app window, the logs or the reports.
- Update signatures and installer checksum verification.

## Supported versions

The latest beta and the latest stable release.

## Verifying an installer

The SHA-256 sum of every installer is in the release notes. How to check it: [FAQ](docs/FAQ.en.md#how-do-i-verify-the-file).
