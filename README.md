# PDR 01 — Астана

Лендинг студии удаления вмятин без покраски (PDR) + админ-панель.

- **Сайт:** https://maqsats.github.io/pdr01-astana/
- **Админка:** https://maqsats.github.io/pdr01-astana/admin.html

## Как это устроено

- `index.html` — лендинг. Весь контент подтягивается из `content.json` при загрузке.
- `content.json` — все тексты, цены, телефоны, фото, FAQ.
- `admin.html` — панель управления: редактирует `content.json` и загружает фото
  напрямую в этот репозиторий через GitHub API. После сохранения GitHub Pages
  пересобирает сайт (~1 минута).

## Доступ к админке

Нужен GitHub personal access token с правом записи в этот репозиторий
(Settings → Developer settings → Personal access tokens). Токен вводится один раз
и хранится только в браузере (localStorage).

## Локальный запуск

```bash
python3 -m http.server 4173
# http://127.0.0.1:4173
```
