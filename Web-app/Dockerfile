# Используйте базовый образ Python
FROM python:3.9-slim

# Устанавливаем рабочую директорию в контейнере
WORKDIR /app

# Копируем зависимости и код в контейнер
COPY requirements.txt .
COPY web-app.py .

# Устанавливаем зависимости
RUN pip install --no-cache-dir -r requirements.txt

# Открываем порт 8000
EXPOSE 8000

# Запускаем приложение при старте контейнера
CMD ["python", "app.py"]
