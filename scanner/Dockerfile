FROM python:3.12-slim

ENV PYTHONDONTWRITEBYTECODE=1 PYTHONUNBUFFERED=1

WORKDIR /app
COPY Python_Scanner.py .

# psycopg2-binary для подключения к Postgres
RUN pip install --no-cache-dir psycopg2-binary

ENTRYPOINT ["python", "Python_Scanner.py"]