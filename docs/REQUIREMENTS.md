# Системные требования / System requirements

[Назад к README](../README.md) · [Back to README](../README.en.md)

Два уровня. **Минимальные:** Тео работает в лёгком режиме, часть функций проще. **Рекомендуемые:** всё включено.
Two levels. **Minimum:** Teo runs in a light mode, some features are simpler. **Recommended:** everything on.

## Windows

| | Минимум / Minimum | Рекомендуем / Recommended |
|---|---|---|
| Система / OS | Windows 10 (1809 и новее) или Windows 11, 64 бита | Windows 11 или Windows 10 22H2, 64 бита |
| Процессор / CPU | 4 потока, набор команд AVX2. Ориентир: Intel Core 8-го поколения и новее, AMD Ryzen | 4 ядра и 8 потоков (Core i5 8-го поколения и новее, Ryzen 5) |
| Память / RAM | 8 ГБ | 16 ГБ |
| Диск / Disk | 3 ГБ свободно | 5 ГБ свободно на SSD |
| Микрофон / Mic | любой рабочий | гарнитура, если в комнате шумно |
| Интернет / Internet | постоянный доступ к Claude | устойчивое соединение |
| Видеокарта / GPU | любая с DirectX 11 | встроенная Intel UHD 620 и новее или отдельная |

Intel Celeron и Pentium 2018 и 2020 годов ниже минимума: у них нет AVX2.
Intel Celeron and Pentium chips from 2018 to 2020 are below the minimum: they lack AVX2.

## macOS

| | Минимум / Minimum | Рекомендуем / Recommended |
|---|---|---|
| Система / OS | macOS 13 и новее | macOS 15 и новее |
| Процессор / CPU | Apple M1 и новее. Mac на Intel не поддерживается | Apple M1 и новее |
| Память / RAM | 8 ГБ | 8 ГБ |
| Диск / Disk | 3 ГБ свободно | 5 ГБ свободно |
| Микрофон / Mic | встроенный подходит | гарнитура в шумной комнате |

macOS спрашивает разрешения по одному, в момент первой нужды: микрофон (обязательно), управление устройством (кнопка Тео, окна, ввод текста), запись экрана, автоматизация и уведомления (по желанию).
macOS asks for permissions one at a time, when first needed: microphone (required), accessibility (Teo key, windows, typing), screen recording, automation and notifications (optional).

## Что ещё нужно / Also needed

- Подписка Claude Pro или выше, или свой ключ API Anthropic. / A Claude Pro or higher subscription, or your own Anthropic API key.
- Для казахского языка и облачного голоса: свой ключ ElevenLabs (по желанию). / For Kazakh and the cloud voice: your own ElevenLabs key (optional).
- Ставить заранее ничего не нужно: ни Python, ни Node. / Nothing to install beforehand: no Python, no Node.

## Как Тео проверяет компьютер / How Teo checks your computer

При первом запуске и по кнопке «Перемерить компьютер» в Настройках: до 10 секунд, без звука и окон. Тео называет один из трёх уровней: рекомендуемый, минимальный, ниже минимума. Бета не начинается на компьютере ниже минимума: Тео честно скажет почему.

On first launch, and with the "Re-measure computer" button in Settings: up to 10 seconds, silent, no windows. Teo names one of three levels: recommended, minimum, below minimum. The trial does not start on a computer below the minimum, and Teo tells you why.
