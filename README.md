# t.fy — скачать / download

**RU** · [English below](#english)

t.fy — набор для чата Twitch: клиент для ПК, расширение для браузера и чат для OBS.
Здесь лежат **только готовые программы**. Скачивать их нужно со страницы
**[Releases](https://github.com/torryfy/tfy-download/releases/latest)**.

| Файл | Что это |
|---|---|
| `tfy-windows-x64.zip` | Клиент t.fy для Windows 10/11 (64-бит) |
| `tfy-extension-chromium.zip` | Расширение для Chrome, Opera, Edge, Brave, Яндекс Браузера |
| `tfy-overlay.zip` | Прозрачный чат для OBS (Browser Source) |
| `SHA256SUMS.txt` | Контрольные суммы файлов |

## Что умеет

- **Баллы t.fy.** Баллы копятся за просмотр стрима, их можно потратить на ★ у ника,
  **переливающийся ник** или **выделенное сообщение** (большой карточкой, в том числе на экране стрима).
- **Свой стиль ника:** 7 готовых наборов (Радуга, Неон, Огонь, Лёд, Золото, Сакура, Кислота) или свои 2–4 цвета,
  4 анимации и 6 шрифтов. Ник выглядит одинаково в клиенте, в браузере (и с 7TV) и в OBS.
- **Клиент для ПК:** темы, русский интерфейс, растягиваемая карточка профиля со стажем подписки,
  базой известных ботов и историей банов, карточки донатов DonationAlerts и DonatePay.
- **Чат для OBS:** прозрачный, смайлы 7TV / BTTV / FFZ, звёздочки, стили ников и покупки за баллы.

## Установка

### Клиент t.fy (Windows)
1. Скачай `tfy-windows-x64.zip` и распакуй в любую папку, например `C:\t.fy`.
2. Запусти `t.fy.exe`.
3. Если Windows покажет синее окно «Windows защитила ваш компьютер», нажми
   **Подробнее → Выполнить в любом случае**. Это обычное окно для программ без платной подписи кода.
4. Войди через Twitch.
5. Для баллов и покупок нужен **ключ t.fy**: его выдаёт стример. Вставь ключ в настройках t.fy
   (вкладка t.fy) или в окошке расширения. Ключ привязывается к твоему аккаунту Twitch.

Обновление: закрой t.fy, распакуй новую версию поверх старой папки. Настройки и вход сохранятся.

### Расширение для браузера
Расширения пока нет в магазине Chrome, поэтому оно ставится вручную:
1. Скачай `tfy-extension-chromium.zip` и **распакуй** в папку, которую не будешь удалять.
2. Открой страницу расширений: `chrome://extensions` (Opera: `opera://extensions`, Edge: `edge://extensions`).
3. Включи **Режим разработчика** (переключатель справа вверху).
4. Нажми **Загрузить распакованное** и выбери распакованную папку (ту, где лежит `manifest.json`).
5. Закрепи значок t.fy на панели браузера и открой чат Twitch.

Обновление: распакуй новую версию в ту же папку и нажми ⟳ на карточке t.fy в списке расширений.

### Чат для OBS
1. Скачай `tfy-overlay.zip` и распакуй, например в `C:\tfy-overlay`.
2. Открой `config.html` в браузере, укажи свой канал и нажми **Скачать config.js**.
   Положи файл в ту же папку.
3. В OBS: **Источники → + → Браузер**, отметь **Локальный файл** и выбери `overlay.html`.
   Ширина 400–480, высота от 220.
4. Посмотреть пример без стрима: добавь к адресу `?demo=1`.

## Безопасность

- Проверить, что файл не подменили, можно по `SHA256SUMS.txt`:
  в PowerShell `Get-FileHash .\tfy-windows-x64.zip` — значение должно совпасть.
- Скачивай t.fy **только отсюда**. Если кто-то присылает «t.fy» с другого сайта, не запускай.
- Программа не просит твой пароль от Twitch: вход идёт через официальную страницу Twitch.
- Все баллы и покупки считает сервер. Изменённая программа не может начислить себе баллы
  или повлиять на чужие: сервер проверяет вход через Twitch, время просмотра, дневные лимиты и частоту запросов.
- Чат для OBS работает без входа и токенов. Токены донатов хранятся только в твоём `config.js`,
  не отправляй этот файл другим.

## Нашёл баг?

Напиши стримеру [torry_fy на Twitch](https://www.twitch.tv/torry_fy): опиши, что делал и что пошло не так,
приложи скриншот.

## Лицензия

Клиент t.fy основан на [Chatterino](https://github.com/Chatterino/chatterino2) (MIT),
текст лицензии лежит в архиве (`LICENSE.txt`). Расширение и чат для OBS распространяются по
[PolyForm Noncommercial 1.0.0](https://polyformproject.org/licenses/noncommercial/1.0.0):
бесплатно для некоммерческого использования.

---

## English

t.fy is a Twitch chat kit: a desktop client, a browser extension and an OBS chat overlay.
This repository holds **ready-to-use programs only** — grab them from
**[Releases](https://github.com/torryfy/tfy-download/releases/latest)**.

| File | What it is |
|---|---|
| `tfy-windows-x64.zip` | t.fy desktop client for Windows 10/11 (64-bit) |
| `tfy-extension-chromium.zip` | Extension for Chrome, Opera, Edge, Brave |
| `tfy-overlay.zip` | Transparent chat for OBS (Browser Source) |
| `SHA256SUMS.txt` | File checksums |

### Features
- **t.fy points** earned by watching: a ★ badge, a **shimmering nick** or a **highlighted message**
  (shown as a big card, on stream too).
- **Your own nick style:** 7 presets or 2–4 custom colors, 4 animations, 6 fonts — the same in the client,
  in the browser (7TV included) and in OBS.
- **Desktop client:** themes, a resizable profile card with sub age, known-bot list and ban history,
  DonationAlerts / DonatePay cards.
- **OBS chat:** transparent, 7TV / BTTV / FFZ emotes, badges, nick styles and point purchases.

### Install
**Client:** unzip `tfy-windows-x64.zip`, run `t.fy.exe`. If SmartScreen appears, click
**More info → Run anyway**. Sign in with Twitch. Points and purchases need a **t.fy key** from the streamer, bound to your Twitch account
(enter it in the t.fy settings tab or in the extension popup). To update, unzip the new version over the old folder.

**Extension:** unzip `tfy-extension-chromium.zip` to a folder you will keep, open `chrome://extensions`
(or `opera://extensions`, `edge://extensions`), turn on **Developer mode**, click **Load unpacked**
and pick the folder with `manifest.json`.

**OBS chat:** unzip `tfy-overlay.zip`, open `config.html`, set your channel, download `config.js` into the same
folder. In OBS add a **Browser** source with **Local file** → `overlay.html` (width 400–480, height 220+).
Add `?demo=1` to preview.

### Security
- Verify downloads against `SHA256SUMS.txt` (`Get-FileHash <file>` in PowerShell).
- Download t.fy **only from here**.
- t.fy never asks for your Twitch password — sign-in goes through Twitch's own page.
- Points and purchases are decided by the server: a modified client cannot grant itself points or touch anyone
  else's — the server checks the Twitch sign-in, watch time, daily caps and request rates.

### License
The client is based on [Chatterino](https://github.com/Chatterino/chatterino2) (MIT; the license is in the zip).
The extension and the OBS chat are under
[PolyForm Noncommercial 1.0.0](https://polyformproject.org/licenses/noncommercial/1.0.0).
