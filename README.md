# Docker: PostgreSQL + File Registry + Python Scanner

## Описание

1. **PostgreSQL** (контейнер `db`) — поднимается в Docker и инициализируется SQL-скриптом.
2. **Таблица 'ops.file_registry'** — создаётся автоматически при первом запуске из 'init-scripts/01_ops_file_registry.sql'.
3. **Python Scanner** (контейнер 'scanner') — рекурсивно проходит по локальному хранилищу файлов и записывает метаданные новых файлов в таблицу 'ops.file_registry'.

## Запуск

- docker compose up -d --build
