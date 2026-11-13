# Teo changelog

[Русская версия](CHANGELOG.md) · [Back to README](README.en.md)

Here are the changes a person will notice. The newest version is on top. Installers and their SHA-256 sums are in [Releases](https://github.com/saint4ai/teo-jarvis/releases).

The Teo interface is in Russian for now, so the Russian names of buttons and sections are given in brackets.

## 1.0.0-beta.1 (November 13, 2026)

The first public beta. 14 days free with every feature, then $10 a month.

What's new:

- A 14-day free trial with every feature. No card needed.
- Sign in to your Teo account with Telegram. One account, one computer.
- Payment inside Teo: Settings («Настройки»), the "Teo account and subscription" section («Аккаунт Тео и подписка»). Two ways: "Pay with a Russian bank card" («Оплата Россия») and "Pay with a card from another country" («Оплата другие страны»), where the payment link arrives by SMS. No automatic charges.
- Beta updates come through a separate beta channel. Teo checks for them once a day.
- A Dashboard with five buttons: Home («Домой»), Work («Дела»), Skills («Навыки»), Connections («Подключения»), Settings («Настройки»). The former fourteen tabs are now inside these five.
- Home: what Teo is doing right now, Claude token usage and ElevenLabs character usage, Claude usage limits on one card, what Teo knows about you, the activity feed and updates.
- Connections: Google Drive and other services through Claude connectors, in four steps, with a "Check the list" button («Проверить список»). Mail with an app password, calendar by link.
- Telegram and WhatsApp: sign in with a QR code or a phone number.
- The Teo browser opens with a start page and comes to the front. Before the first launch Teo warns you that it does everything in this browser on your behalf.
- Work: Claude Code agent monitoring is on by default. You see which agents are working and which are waiting for you.
- Settings: the Claude sign-in no longer asks you to press the button a second time. The "Where Teo gets stuck" block («Где Тео спотыкается») comes first, and a red dot on the button shows a problem.
- The "Male 5" on-device voice («Мужской 5») is the default and free. ElevenLabs works only with your own key.
- Teo does not react to its own voice. You can stop it with the Teo key (Pause on Windows, right Option on Mac) or with the "Stop" button («Остановить») in the capsule.
- Videos on websites: pause, resume, next episode and full screen.
- Teo errors go to the developers automatically, without your conversations, files or keys. The switch is in Settings. Next to it is the "Send feedback" form («Оставить отзыв»).

Known issues, not fixed yet:

- You cannot stop Teo by voice while it is speaking: the microphone does not listen at that time.
- The installers do not have a paid signature yet. Windows and macOS warn about an unknown publisher. What to click: [FAQ](docs/FAQ.en.md#installing), and for Mac the [guide with screenshots](docs/INSTALL-MAC.en.md).
- We do not promise Gmail through the Claude connector yet. Gmail, Yandex Mail and Mail.ru connect with an app password.
- Macs with Intel processors are not supported. The Mac image is added to the release separately from the Windows installer.
