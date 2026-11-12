# Безопасность / Security

## Как сообщить об уязвимости / Reporting a vulnerability

Нашёл уязвимость в Тео? Не создавай публичный Issue.

1. Открой вкладку **Security** этого репозитория и нажми **Report a vulnerability**. Сообщение увидят только разработчики.
2. Опиши, что нашёл, как это повторить и что может случиться.
3. Не прикладывай ключи, пароли и чужие личные данные.

Found a vulnerability in Teo? Do not open a public issue.

1. Open the **Security** tab of this repository and click **Report a vulnerability**. Only the developers see the report.
2. Describe what you found, how to reproduce it and what can happen.
3. Do not attach keys, passwords or other people's personal data.

## На что мы смотрим особенно / What we care about most

- Чужой текст (чаты, почта, сайты, файлы) не должен управлять Тео.
- Отправка сообщений, закрытие программ и чистка идут только после «да» человека.
- Ключи и входы не попадают в окно программы, журнал и отчёты.
- Подпись обновлений и проверка суммы установщика.

- Foreign text (chats, mail, websites, files) must never steer Teo.
- Sending messages, closing apps and cleanup need a human "yes".
- Keys and sign-ins must not reach the app window, logs or reports.
- Update signature and installer checksum verification.

## Какие версии поддерживаем / Supported versions

Последняя бета и последняя стабильная версия. / The latest beta and the latest stable release.

## Как проверить установщик / Verifying an installer

Сумма SHA-256 каждого установщика записана в описании выпуска. Инструкция: [FAQ](docs/FAQ.md#как-проверить-что-файл-настоящий). / Every installer has a SHA-256 sum in the release notes. See the [FAQ](docs/FAQ.en.md#how-do-i-verify-the-file).
