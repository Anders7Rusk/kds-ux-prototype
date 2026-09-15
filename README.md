# KDS — витрина UX-доработок

Статичный прототип: разбор доработок экрана кухни (KDS) — 30 сценариев,
переключение «Как сейчас / Как лучше», режим показа слайдами.

## Как открыть

- **Локально:** скачать папку и открыть `ux-proposals.html` в браузере (Chrome).
  Сервер не нужен; для шрифтов и стилей ДС нужен интернет.
- **GitHub Pages:** корневой `index.html` перенаправляет на витрину
  (после включения Pages ссылка вида `https://<логин>.github.io/kds-ux-prototype/`).

## Файлы

| Файл | Что это |
|------|---------|
| `ux-proposals.html` | Витрина: меню доработок, описание, планшет с экраном, ревью, режим показа |
| `kds-screen.html` | Сам экран KDS со всеми демо-сценариями (`?embed=1` — без корпуса планшета) |
| `index.html` | Редирект на витрину (для GitHub Pages) |

## Обновление из рабочего воркспейса

Исходники живут в `…\GitHub\DS\iiko-ds-prototypes\KDS\`. Чтобы обновить витрину:

```powershell
Copy-Item ..\DS\iiko-ds-prototypes\KDS\ux-proposals.html . -Force
Copy-Item ..\DS\iiko-ds-prototypes\KDS\kds-screen.html . -Force
git add -A
git commit -m "обновление витрины"
git push
```

## Публикация (один раз)

1. Создать репозиторий на GitHub (например, `kds-ux-prototype`, приватный).
2. Привязать и запушить:
   ```powershell
   git remote add origin https://github.com/<логин>/kds-ux-prototype.git
   git push -u origin main
   ```
3. Включить Pages: **Settings → Pages → Deploy from a branch → main / (root)**.
   Через 1–2 минуты витрина откроется по адресу `https://<логин>.github.io/kds-ux-prototype/`.

> Внимание: GitHub Pages для приватных репозиториев доступен на платных планах
> (Pro / Team / Enterprise). Для публичного репозитория витрину выкладывать только
> с разрешения — материалы внутренние.
