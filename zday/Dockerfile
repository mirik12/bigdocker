FROM python:3

# Створюємо робочу директорію в контейнері
WORKDIR /opt/zday

# Копіюємо requirements.txt у контейнер
COPY requirements.txt .

# Встановлюємо залежності Python
RUN pip3 install -r requirements.txt

# Копіюємо всі файли з поточної директорії (де знаходиться Dockerfile) у контейнер
COPY . .

EXPOSE 8000

CMD ["python3", "manage.py", "runserver", "0.0.0.0:8000"]
