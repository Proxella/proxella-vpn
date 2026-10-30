# Proxella VPN — для Windows 7, 8, 10, 11, Android и macOS

**Proxella** — VPN-сервис со своими приложениями для компьютера, телефона и Mac.
Для **Windows 7 и Windows 8 / 8.1** есть отдельная сборка: она запускается там, где многие
VPN-программы уже не поддерживаются.

- 🌐 Сайт: **[proxella.pro](https://proxella.pro/#github)**
- ⬇️ Скачать: **[proxella.pro/zagruzka](https://proxella.pro/zagruzka#github)** или из
  [последнего релиза](https://github.com/Proxella/proxella-vpn/releases/latest) этого репозитория
- 🍏 Mac: [proxella.pro/skachat/macos](https://proxella.pro/skachat/macos#github)
- 🎁 Пробный период — сразу после установки, без карты и регистрации

## Скачать

| Система | Скачать | Зеркало на GitHub | Для каких устройств |
|---|---|---|---|
| **Windows 7, 8, 8.1** | [ProxellaLegacySetup-1.4.119.exe](https://proxella.pro/downloads/ProxellaLegacySetup-1.4.119.exe?utm_source=github&utm_medium=readme) | [скачать](https://github.com/Proxella/proxella-vpn/releases/latest/download/ProxellaLegacySetup-1.4.119.exe) | отдельная сборка для старых Windows |
| **Windows 10, 11** | [ProxellaSetup-0.5.101.exe](https://proxella.pro/downloads/ProxellaSetup-0.5.101.exe?utm_source=github&utm_medium=readme) | [скачать](https://github.com/Proxella/proxella-vpn/releases/latest/download/ProxellaSetup-0.5.101.exe) | обычные компьютеры и ноутбуки |
| **Android** | [Proxella-android-0.3.33-arm64.apk](https://proxella.pro/downloads/Proxella-android-0.3.33-arm64.apk?utm_source=github&utm_medium=readme) | [скачать](https://github.com/Proxella/proxella-vpn/releases/latest/download/Proxella-android-0.3.33-arm64.apk) | большинство телефонов и Android TV |
| **Android, старые телефоны** | [Proxella-android-0.3.33-arm.apk](https://proxella.pro/downloads/Proxella-android-0.3.33-arm.apk?utm_source=github&utm_medium=readme) | [скачать](https://github.com/Proxella/proxella-vpn/releases/latest/download/Proxella-android-0.3.33-arm.apk) | если пишет «несовместимо с CPU_ABI устройства» |
| **macOS 12 Monterey и новее** | [Proxella-0.1.7.pkg](https://proxella.pro/downloads/Proxella-0.1.7.pkg?utm_source=github&utm_medium=readme) | [скачать](https://github.com/Proxella/proxella-vpn/releases/latest/download/Proxella-0.1.7.pkg) | все Mac с Apple Silicon (M1 и новее) и Intel примерно с 2015 года |
| **macOS 11 Big Sur** | [Proxella-Legacy-0.1.7.pkg](https://proxella.pro/downloads/Proxella-Legacy-0.1.7.pkg?utm_source=github&utm_medium=readme) | [скачать](https://github.com/Proxella/proxella-vpn/releases/latest/download/Proxella-Legacy-0.1.7.pkg) | Mac на Intel 2013–2014 годов и Mac, оставшиеся на Big Sur |

После установки приложение само обновляется до свежей версии.
Колонка «Скачать» ведёт на сайт [proxella.pro](https://proxella.pro/zagruzka#github), «Зеркало на GitHub» — на те же файлы
в релизе этого репозитория: пригодится, если сайт не открывается. Контрольные суммы — в конце страницы.

## VPN для Windows 7: почему многие не запускаются

Microsoft прекратила поддержку Windows 7 в январе 2020 года, и разработчики постепенно перестали
собирать под неё программы: новые версии многих VPN-клиентов требуют Windows 10 или 11.
На Windows 7 такие программы обычно не ставятся или падают с ошибкой вроде:

- «Запуск программы невозможен, так как на компьютере отсутствует **api-ms-win-core-…dll**»;
- «Точка входа в процедуру … не найдена в библиотеке **KERNEL32.dll**»;
- «Это приложение не поддерживает текущую версию Windows».

У Proxella для Windows 7 и 8 своя сборка — **ProxellaLegacySetup**. Её не нужно искать отдельно:
страница [proxella.pro/zagruzka](https://proxella.pro/zagruzka#github) сама определяет версию Windows и
предлагает нужный файл.

## Как установить на Windows 7

1. Скачайте [ProxellaLegacySetup-1.4.119.exe](https://proxella.pro/downloads/ProxellaLegacySetup-1.4.119.exe?utm_source=github&utm_medium=readme).
2. Браузер может написать, что файл «скачивают редко». Это не сообщение об угрозе: приложение
   новое и пока без цифровой подписи, поэтому такое предупреждение видят все. Нажмите «Сохранить».
3. Запустите установщик. Если Windows спросит про неизвестного издателя — разрешите запуск.
4. Откройте Proxella и подключитесь. Пробный период включится сам, на Windows 7 и 8 — сутки.

На Windows 10 и 11 всё так же, только файл другой — `ProxellaSetup-0.5.101.exe`.

## Если на Windows 7 не открываются сайты

Это частая беда старых систем, и она не связана с VPN. Обычно помогает:

- **Проверить дату и время.** Если часы сбились, браузер пишет «Ваше подключение не защищено».
- **Поставить обновления сертификатов и протоколов**: KB4474419 (поддержка SHA-2),
  KB4490628 (обновление стека обслуживания) и KB3140245 (TLS 1.1 и 1.2 по умолчанию) —
  они есть в каталоге Центра обновления Microsoft.
- **Обновить браузер.** Последняя версия Google Chrome для Windows 7 и 8.1 — 109. Если сайты
  ругаются на сертификаты, попробуйте браузер, который ещё обновляется под Windows 7.

## Тарифы

| Тариф | Цена | Устройств одновременно | Трафик в месяц |
|---|---|---|---|
| **Личная** | 299 ₽ в месяц · 1 620 ₽ за полгода · 2 700 ₽ за год | 2 | 500 ГБ |
| **Семейная** | 600 ₽ в месяц · 3 240 ₽ за полгода · 5 400 ₽ за год | 10 | 2 500 ГБ |

- **Пробный период:** 2 дня (на Windows 7 и 8 — сутки), без карты и регистрации.
  За подтверждение почты — ещё 3 дня.
- **Оплата:** банковские карты РФ через ЮKassa, чек приходит на почту.
- Актуальные цены — на [proxella.pro/tarify](https://proxella.pro/tarify#github).

## Частые вопросы

**Какой впн работает на виндовс 7?** Proxella: для Windows 7 и 8 у неё отдельная сборка —
[ProxellaLegacySetup-1.4.119.exe](https://proxella.pro/downloads/ProxellaLegacySetup-1.4.119.exe?utm_source=github&utm_medium=readme).
Пробный период — сутки, без карты и регистрации.

**Есть ли впн для макбука?** Да. Для macOS 12 и новее —
[Proxella-0.1.7.pkg](https://proxella.pro/downloads/Proxella-0.1.7.pkg?utm_source=github&utm_medium=readme),
для macOS 11 Big Sur — [Proxella-Legacy-0.1.7.pkg](https://proxella.pro/downloads/Proxella-Legacy-0.1.7.pkg?utm_source=github&utm_medium=readme).
Подробнее — на [proxella.pro/skachat/macos](https://proxella.pro/skachat/macos#github).

**Где скачать впн для пк?** На [proxella.pro/zagruzka](https://proxella.pro/zagruzka#github): страница сама определит
версию Windows и предложит нужный файл. Здесь те же файлы — в [последнем релизе](https://github.com/Proxella/proxella-vpn/releases/latest).

**Нужна ли регистрация?** Нет. Пробный период начинается сразу после установки. Почту можно
указать позже — за это добавится 3 дня.

**Можно ли одной подпиской подключить компьютер и телефон?** Да. «Личная» — 2 устройства
одновременно, «Семейная» — 10: Windows, Android, Mac и Android TV на одном аккаунте.

**Есть ли версия для iPhone и iPad?** На iPhone и iPad Proxella работает через бесплатное
приложение INCY из App Store. Подключение — на [proxella.pro](https://proxella.pro/#github).

**Работает ли на телевизоре?** На телевизорах с Android TV и Google TV — через приложение для
Android. Инструкция — [proxella.pro/vpn-dlya-televizora](https://proxella.pro/vpn-dlya-televizora#github).

**Безопасно ли скачивать отсюда?** Здесь лежат те же файлы, что раздаёт сайт. Сверить их можно по
контрольным суммам ниже.

**Куда писать, если не получилось?** На [proxella.pro/kontakty](https://proxella.pro/kontakty#github).

## Контрольные суммы (SHA-256)

```
1343c3ec529863ee92bd62d52147207440b506f602def2a79ce2da634accc327  ProxellaLegacySetup-1.4.119.exe
134966d77e94a678f1e2d055cae9249d11a7388df3661c0d3a28b98477808a83  ProxellaSetup-0.5.101.exe
278ddbd1a387b630f67910f2c53a8c8e77e06888fde87360153c0aea4b4aa014  Proxella-android-0.3.33-arm64.apk
7ba2e3a10b0eea8565080211c07b4031c65ce890cef0666ae16ba063f19e746c  Proxella-android-0.3.33-arm.apk
9ba207ba6b10b04fdedefb30dcd7ba3d7b3118d72b4456deca2c940b9f880ccb  Proxella-0.1.7.pkg
4b5ed1e9e0f966d7d35b01ad4c3b61facd8678c27ede252a8fdeba5cbc26efd6  Proxella-Legacy-0.1.7.pkg
```

Проверить на Windows: `certutil -hashfile ProxellaLegacySetup-1.4.119.exe SHA256`.
На Mac: `shasum -a 256 Proxella-0.1.7.pkg`.

---

Официальная страница для скачивания Proxella. Исходный код приложений закрыт.
Сайт сервиса — [proxella.pro](https://proxella.pro/#github).
