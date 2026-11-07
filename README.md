# site_CICD

Статическая веб-страница с автоматическим деплоем через GitHub Actions.

## Статус сборки

![Deploy workflow status](https://github.com/rinnlv/site_CICD/actions/workflows/deploy.yml/badge.svg)

## Структура проекта

- `index.html` — основная страница
- `style.css` — стили
- `pic1.jpg` – `pic6.jpg` — изображения
- [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml) — CI/CD workflow для деплоя

## Как это работает

При каждом push в репозиторий запускается GitHub Actions workflow
[`deploy.yml`](.github/workflows/deploy.yml), который автоматически
выполняет сборку и деплой сайта. Текущее состояние последнего запуска
отображается в статус-бейдже выше:

- 🟢 **passing** — последняя сборка прошла успешно
- 🔴 **failing** — последняя сборка завершилась с ошибкой
- 🟡 **running** — workflow выполняется в данный момент
- ⚪ **no status** — workflow ещё не запускался
