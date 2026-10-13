# 🏦 Loan Approval Service

Учебное приложение команды «ГИК МАСТЕРС»: обучение модели для прогноза одобрения кредита, FastAPI и веб-интерфейс.

**Команда:** Андрей Сырчин — backend и CI/CD; Артём Мастеров — ML и frontend.

## Структура

`backend/` — API, обучение, данные и тесты; `frontend/` — HTML/CSS/JS; `docs/` — исходное описание вклада участников.

## Запуск

```sh
cd backend
uv sync
uv run python ml/train.py
uv run uvicorn api.main:app --reload
```

Веб-интерфейс и API: `http://127.0.0.1:8000`. Обучение создаёт локальные артефакты модели. Требования и детали: [backend/README.md](backend/README.md).

Учебный сервис не предназначен для реального принятия кредитных решений. Загружайте только доверенные сериализованные модели: pickle/joblib могут выполнять код при загрузке.

Перенесено из [geek-masters/ml-service](https://sourcecraft.dev/geek-masters/ml-service). [Исходное описание команды](docs/source-readme.md) сохранено. SourceCraft CI остаётся конфигурацией источника и не запускается на GitHub.
