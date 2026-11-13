# Что Тео делает с данными / What Teo does with your data

[Назад к README](../README.md) · [Back to README](../README.en.md)

Это краткое описание. Полная политика конфиденциальности на сервере Тео: [teo.onai.academy/privacy](https://teo.onai.academy/privacy), есть казахская версия.
This is a short description. The full privacy policy is on the Teo server: [teo.onai.academy/privacy](https://teo.onai.academy/privacy), a Kazakh version is available.

## По-русски

Тео живёт на твоём компьютере. Память, переписки, журнал и ключи лежат у тебя. Наружу уходит только то, что нужно для ответа.

### Что остаётся на компьютере

- Память Тео: что ты просил запомнить, профиль из знакомства.
- Журнал ходов и заметки о сбоях.
- Переписки Telegram и WhatsApp, которые ты подключил, и голосовые из них.
- Ключи сервисов в Диспетчере учётных данных Windows или в Связке ключей macOS.
- Вход в Claude делает сама программа Claude. Тео ключ подписки не видит и не хранит.
- Распознавание речи и голос «Мужской 5» работают на компьютере.

Срок хранения можно задать, тогда старое стирается само. Без срока Тео ничего не удаляет.

### Что уходит с компьютера

| Куда | Что | Когда | Как отключить |
|---|---|---|---|
| Claude (Anthropic) | То, что ты сказал. Куски файлов, писем, страниц и сообщений, к которым ты попросил обратиться. Снимок окна по клавише «Объяснить экран» | В каждом ответе | Целиком нельзя: на этом строится работа. Можно не подключать почту и чаты и не просить читать файлы и экран |
| ElevenLabs | Текст ответа, чтобы озвучить. Звук речи при диктовке по-казахски | Только если ты выбрал облачный голос или казахский и ввёл свой ключ | Выбрать «Голос на компьютере» или «Только текст» |
| Hugging Face | Ничего твоего. Скачиваются модели | Один раз при первом запуске | Нельзя без потери распознавания речи |
| GitHub | Ничего твоего. Тео раз в сутки спрашивает описание версии и скачивает обновление | Через 10 минут после запуска и раз в сутки | Выключается настройкой обновлений |
| Сервер аккаунта Тео | Номер аккаунта в Telegram, даты подписки и пробного периода, версия Тео, число просьб по дням без их текста. Отпечатки телефона и компьютера, но не сами значения | При входе и раз в сутки | Удалить аккаунт на странице аккаунта |
| Сервер разработчиков | Ошибки и сбои Тео без разговоров, файлов и ключей | Автоматически в бете | Выключатель в Настройках, блок «Приватность» |
| Сервер разработчиков | Отчёт для поддержки и отзыв | Только по твоей кнопке | Не нажимать |

### Чего Тео не делает

- Не шлёт разговоры, файлы и переписки на сервер разработчиков.
- Не хранит ключи в открытом виде и не отдаёт их окну программы.
- Не выполняет как команду текст из чатов, почты, сайтов и файлов.
- Не отправляет сообщения, не закрывает программы и не чистит файлы без твоего «да».

## In English

Teo lives on your computer. Memory, chats, logs and keys stay with you. Only what is needed for an answer leaves the machine.

### Stays on your computer

- Teo memory: what you asked it to remember, the profile from the intro.
- The turn log and crash notes.
- Telegram and WhatsApp chats you connected, with their voice messages.
- Service keys in Windows Credential Manager or macOS Keychain.
- The Claude app itself handles the Claude sign-in. Teo never sees or stores your subscription key.
- Speech recognition and the "Мужской 5" voice run on the computer.

You can set a retention period and old data is erased automatically. Without one, Teo deletes nothing.

### Leaves your computer

| To | What | When | How to turn off |
|---|---|---|---|
| Claude (Anthropic) | What you said. Parts of files, mail, pages and messages you asked Teo to open. A window snapshot when you use "Explain screen" | Every answer | Cannot be turned off: Teo runs on it. You can skip mail and chats and avoid asking for files or screen |
| ElevenLabs | Answer text for the voice. Speech audio for Kazakh dictation | Only if you chose the cloud voice or Kazakh and entered your own key | Pick "On-device voice" or "Text only" |
| Hugging Face | Nothing of yours. Models are downloaded | Once, on first launch | Not possible without losing speech recognition |
| GitHub | Nothing of yours. Once a day Teo asks for the version description and downloads updates | 10 minutes after launch, then daily | Update setting |
| Teo account server | Your Telegram account number, trial and subscription dates, Teo version, request counts per day without their text. Fingerprints of phone and computer, not the raw values | At sign-in and daily | Delete the account on the account page |
| Developer server | Teo errors and crashes without conversations, files or keys | Automatically in the beta | Switch in Settings, block "Privacy" |
| Developer server | Support report and feedback | Only when you press the button | Do not press |

### What Teo does not do

- Does not send conversations, files or chats to the developer server.
- Does not store keys in plain text or give them to the app window.
- Does not run text from chats, mail, websites or files as a command.
- Does not send messages, close apps or clean files without your "yes".
