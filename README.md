# 🏦 Loan Approval Service

Самостоятельный учебный проект Артёма Мастерова: обучение модели для прогноза одобрения кредита, FastAPI и веб-интерфейс.

**Автор:** Артём Мастеров. Проект разработан самостоятельно.

## Структура

`backend/` — API, обучение, данные и тесты; `frontend/` — HTML/CSS/JS; `docs/` — подробное описание проекта.

## Запуск

```sh
cd backend
uv sync
uv run python ml/train.py
uv run uvicorn api.main:app --reload
```

Веб-интерфейс и API: `http://127.0.0.1:8000`. Обучение создаёт локальные артефакты модели. Требования и детали: [backend/README.md](backend/README.md).

Учебный сервис не предназначен для реального принятия кредитных решений. Загружайте только доверенные сериализованные модели: pickle/joblib могут выполнять код при загрузке.

Перенесено из [geek-masters/ml-service](https://sourcecraft.dev/geek-masters/ml-service). [Подробное описание проекта](docs/source-readme.md). SourceCraft CI остаётся конфигурацией источника и не запускается на GitHub.
