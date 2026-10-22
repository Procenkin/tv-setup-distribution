# Настройка ТВ — сборки

Здесь публикуются готовые сборки приложения «Настройка ТВ»: оно убирает рекламу и слежку производителя
с Android TV и ставит чистый домашний экран. Без ИИ-агентов, терминала и компьютерных навыков.

**Скачать:** https://tv.pereplet.space/ — страница продукта с инструкциями.
Те же файлы — в разделе [Releases](https://github.com/Procenkin/tv-setup-distribution/releases),
последняя версия — [здесь](https://github.com/Procenkin/tv-setup-distribution/releases/latest).

## Какой файл выбрать

| Файл | Для чего |
|---|---|
| `tv-setup-<версия>-arm64-v8a.apk` | большинство телефонов на Android 8+ |
| `tv-setup-<версия>-armeabi-v7a.apk` | старые 32-битные телефоны и многие телевизоры |
| `tv-setup-<версия>-universal.apk` | если не знаете, что выбрать (больше по размеру) |
| `tv-setup-<версия>-x86_64.apk` | эмуляторы и редкие x86-устройства |
| `SHA256SUMS.txt` | контрольные суммы всех файлов |

Обновления приходят внутри приложения: кнопка «Обновить» скачивает новую версию отсюда и сверяет
контрольную сумму перед установкой.

## Проверить файл вручную

```bash
sha256sum -c SHA256SUMS.txt --ignore-missing
```

## Совместимость

Android TV и Google TV на Android 8.0 и новее с включённой «Отладкой по USB». Samsung (Tizen),
LG (webOS) и Amazon Fire TV не поддерживаются.

Домашний экран основан на открытом проекте [CleanYourTV](https://github.com/Gathin23/cleanyourtv)
(MIT). Android TV и Google TV — товарные знаки Google LLC; проект с Google не связан.
