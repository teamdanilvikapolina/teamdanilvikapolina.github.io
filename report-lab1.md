# Отчёт по лабораторной работе 1

**Сайт команды:** https://teamdanilvikapolina.github.io/

**Репозиторий:** https://github.com/teamdanilvikapolina/teamdanilvikapolina.github.io

## Состав команды и роли

| Участник | Роль | Отвечает за |
|----------|------|-------------|
| Данил | Разработчик | Репозиторий, HTML, `robots.txt`, `sitemap.xml` |
| Вика | Автор | Текст страницы о квазибуплоне |
| Полина | Аналитик | Проверка сайта, Вебмастер, Search Console, журнал экспериментов |

## Структура сайта

- `index.html` — главная страница: название команды, описание проекта, ссылка на страницу о квазибуплоне
- `chto-takoe-kvazibuplon.html` — страница о квазибуплоне (300 слов, 4 подраздела `h2`, пометка об учебном эксперименте)
- `robots.txt` — запрет `/drafts/`, ссылка на `sitemap.xml`
- `sitemap.xml` — 2 URL: главная (`/`) и страница о квазибуплоне
- `.nojekyll` — отключает Jekyll
- `362026b6893d0e6cabbc73aa4efd0014.txt` — файл ключа IndexNow
- `journal.md` — журнал экспериментов
- `drafts/` — скриншоты проверок (закрыты от индексации через `robots.txt`)

## Чек-лист разметки (задание 4)

| Пункт | index.html | chto-takoe-kvazibuplon.html |
|-------|-----------|------------------------------|
| `<html lang="ru">` | да | да |
| `title` уникален, ≤ 60–70 символов | 63 символа | 44 символа |
| `meta description` описывает страницу | 143 символа | 137 символов |
| Ровно один `h1` | да | да |
| `canonical` = адрес этой страницы | `https://teamdanilvikapolina.github.io/` | `https://teamdanilvikapolina.github.io/chto-takoe-kvazibuplon.html` |
| Текст виден в исходном коде без JavaScript | да (без JS) | да (без JS) |
| Пометка об учебном эксперименте | да | да |
| Ссылка с главной | — | да |

## Скриншоты проверок

*(заполняются после проверок в Вебмастере и Search Console, сохраняются в `drafts/`)*

- [ ] Анализ `robots.txt` в Яндекс Вебмастере — без ошибок
- [ ] Анализ `sitemap.xml` в Яндекс Вебмастере — без ошибок, 2 URL
- [ ] Проверка ответа сервера — 200 без редиректа
- [ ] Подтверждение прав мета-тегом в Яндекс Вебмастере
- [ ] Подтверждение прав HTML-тегом в Google Search Console
- [ ] Статус отправленного `sitemap.xml` в обоих сервисах
- [x] Ответ IndexNow `200`/`202` — получен **202** `{"success":true}` 2026-10-08
  (запрос: `https://yandex.com/indexnow?url=…/chto-takoe-kvazibuplon.html&key=362026b6893d0e6cabbc73aa4efd0014`,
  аналогично для главной страницы)

## Результаты авто-проверки 2026-10-08

Проверено прямым запросом к опубликованному сайту:

| URL | Код ответа |
|-----|-----------|
| `https://teamdanilvikapolina.github.io/` | 200 |
| `https://teamdanilvikapolina.github.io/chto-takoe-kvazibuplon.html` | 200 (без редиректа) |
| `https://teamdanilvikapolina.github.io/robots.txt` | 200 |
| `https://teamdanilvikapolina.github.io/sitemap.xml` | 200 |
| `https://teamdanilvikapolina.github.io/362026b6893d0e6cabbc73aa4efd0014.txt` | 200 |
| IndexNow (обе страницы) | 202 `{"success":true}` |

## Журнал экспериментов

Первая запись: [journal.md](journal.md) — 2026-10-08, гипотеза в числах
(Яндекс — 7 дней, Google — 14 дней).

## Статус

- [x] Сайт открывается по HTTPS в корне домена
- [x] Главная и страница о квазибуплоне опубликованы
- [x] `robots.txt` и `sitemap.xml` на месте, sitemap указан в `robots.txt`
- [x] Ключ IndexNow опубликован
- [x] Уведомление IndexNow отправлено — 202 (обе страницы)
- [x] Журнал экспериментов с первой записью
- [ ] Скриншоты Вебмастера и Search Console
- [ ] Скриншот ответа IndexNow
- [ ] Адрес сайта и состав команды сообщены преподавателю
