FROM python:3.9

# Устанавливаем переменную окружения PYTHONUNBUFFERED для вывода немедленной информации stdout/stderr
ENV PYTHONUNBUFFERED=1

# Устанавливаем переменную окружения PYTHONUNBUFFERED для вывода немедленной информации stdout/stderr
ENV PYTHONUNBUFFERED=1

# Копируем зависимости проекта в контейнер
COPY requirements.txt .

# Копируем исходный код проекта в контейнер
COPY web.py .


# запуск pipenv
#ENTRYPOINT ["pipenv", "run", "python", "configure_and_run.py", "&"]

# Запускаем команду для запуска веб-сервера
CMD ["uvicorn", "web.py:app", "--host", "0.0.0.0", "--port", "8000"]