<p align="center">
  <img src="assets/vseti-banner.png" width="100%" alt="Vseti">
</p>

<h1 align="center">Vseti Desktop</h1>

<p align="center">
  Десктопное приложение Vseti для Windows, macOS и Linux
</p>

<p align="center">
  <a href="https://github.com/KinoVestnik/Vseti-desktop/releases/latest"><img src="https://img.shields.io/github/v/release/KinoVestnik/Vseti-desktop?style=for-the-badge&logo=github&label=Версия" alt="Последняя версия"></a>
  <a href="https://github.com/KinoVestnik/Vseti-desktop/releases"><img src="https://img.shields.io/github/downloads/KinoVestnik/Vseti-desktop/total?style=for-the-badge&logo=github&label=Загрузки" alt="Загрузки"></a>
  <a href="LICENSE"><img src="https://img.shields.io/github/license/KinoVestnik/Vseti-desktop?style=for-the-badge&label=Лицензия" alt="GPL-2.0"></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Windows-x64%20%7C%20x86%20%7C%20ARM64-0078D4?style=flat-square&logo=windows11&logoColor=white" alt="Windows">
  <img src="https://img.shields.io/badge/macOS-Intel%20%7C%20Apple%20Silicon-000000?style=flat-square&logo=apple&logoColor=white" alt="macOS">
  <img src="https://img.shields.io/badge/Linux-AppImage%20%7C%20DEB%20%7C%20RPM-FCC624?style=flat-square&logo=linux&logoColor=111111" alt="Linux">
</p>

Vseti Desktop открывает [`vseti.click`](http://vseti.click/) в отдельном приложении, запоминает состояние окна и предоставляет системную интеграцию, полноэкранный режим, поддержку внешних плееров и TorrServer.

> [!TIP]
> Для большинства компьютеров с Windows выбирайте установщик **x64** в [последнем релизе](https://github.com/KinoVestnik/Vseti-desktop/releases/latest).

## Скачать

| Платформа | Устройство | Файл в релизе |
|---|---|---|
| Windows | Большинство компьютеров, 64-bit | `vseti-x64-<версия>.exe` |
| Windows | Старые 32-битные компьютеры | `vseti-ia32-<версия>.exe` |
| Windows | Устройства Windows ARM | `vseti-arm64-<версия>.exe` |
| macOS | Mac на Intel | `vseti-x64-<версия>.dmg` |
| macOS | Mac на Apple Silicon | `vseti-arm64-<версия>.dmg` |
| Linux | Универсальный запуск x64 | `vseti-x86_64-<версия>.AppImage` |
| Linux | Debian, Ubuntu и производные | `vseti-amd64-<версия>.deb` |
| Linux | Fedora, RHEL и производные | `vseti-x86_64-<версия>.rpm` |
| Linux ARM64 | Debian/Ubuntu или Fedora/RHEL | `arm64.deb` или `aarch64.rpm` |

Все установщики, контрольные суммы SHA-256 и архив соответствующего исходного кода находятся в разделе **[Releases](https://github.com/KinoVestnik/Vseti-desktop/releases)**.

## Установка

<details open>
<summary><strong>Windows</strong></summary>

1. Скачайте установщик своей архитектуры. Обычно нужен файл с `x64` в названии.
2. Закройте запущенную версию Vseti и откройте скачанный `.exe`.
3. Подтвердите запрос контроля учётных записей Windows.
4. Запустите **Vseti** с рабочего стола или из меню «Пуск».

Новая версия устанавливается поверх предыдущей: удалять старую Vseti не требуется. Пакеты пока не подписаны коммерческим сертификатом, поэтому Windows может показать предупреждение SmartScreen.

</details>

<details>
<summary><strong>macOS</strong></summary>

1. Выберите DMG для Intel или Apple Silicon.
2. Откройте образ и перенесите **Vseti** в папку `Applications`.
3. При обновлении подтвердите замену существующего приложения.

Сборки пока не нотаризованы Apple. Если macOS блокирует первый запуск, разрешите приложение в **System Settings → Privacy & Security**.

</details>

<details>
<summary><strong>Linux</strong></summary>

AppImage:

```bash
chmod +x vseti-x86_64-<версия>.AppImage
./vseti-x86_64-<версия>.AppImage
```

DEB:

```bash
sudo apt install ./vseti-amd64-<версия>.deb
```

RPM:

```bash
sudo rpm -Uvh vseti-x86_64-<версия>.rpm
```

</details>

## Пульт

Управлять интерфейсом можно с телефона, планшета или другого устройства через браузер.

| Режим | Ссылка | Назначение |
|---|---|---|
| Веб-пульт | [Открыть пульт](http://vseti.click/remotecontrol/remotecontrol.html) | Навигация, выбор, возврат и управление воспроизведением |
| Экранная клавиатура | [Открыть клавиатуру](http://vseti.click/remotecontrol/keyboard.html) | Удобный ввод текста и поисковых запросов |

При запросе авторизации войдите в свой аккаунт Vseti. Для быстрого доступа страницу пульта можно добавить на главный экран телефона.

## Горячие клавиши в приложении

| Клавиша | Действие |
|---|---|
| <kbd>F</kbd> | Включить или выключить полноэкранный режим |
| <kbd>S</kbd> | Открыть поиск |
| <kbd>M</kbd> | Открыть или закрыть боковое меню |
| <kbd>Alt</kbd> + <kbd>F4</kbd> | Закрыть приложение |

Горячие клавиши не перехватываются во время ввода текста, кроме системного сочетания закрытия приложения.

## Возможности

- единое приложение для Windows, macOS и Linux;
- стартовая страница `http://vseti.click/` и возможность указать собственный URL;
- сохранение размера, положения окна и полноэкранного режима;
- интеграция с VLC, KMPlayer, MPC-HC, MPC-BE и MPC-QT на поддерживаемых системах;
- встроенная поддержка TorrServer;
- экспорт и импорт пользовательских настроек;
- проверка новой версии через публичные релизы GitHub.

## Обновление

Автоматическая установка обновлений пока отключена. Для обновления скачайте новый пакет той же архитектуры из [Releases](https://github.com/KinoVestnik/Vseti-desktop/releases/latest) и установите его поверх текущей версии. Пользовательские настройки сохраняются.

## Авторы и исходные проекты

- Автор и сопровождение Vseti Desktop: [KinoVestnik](https://github.com/KinoVestnik)
- Оригинальный проект: 👉 [Kolovatoff/lampa-desktop](https://github.com/Kolovatoff/lampa-desktop)
- Исходный код самой Lampa доступен здесь: 👉 [yumata/lampa-source](https://github.com/yumata/lampa-source)

## Лицензия

Vseti Desktop распространяется по лицензии [GNU GPL-2.0](LICENSE). Архив исходного кода, соответствующий опубликованным сборкам, прикладывается к каждому релизу.
