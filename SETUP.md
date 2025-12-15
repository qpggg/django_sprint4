# Инструкция по запуску проекта Django Blogicum

## Требования
- Python 3.8+
- pip
- venv (встроен в Python 3.3+)

## Шаги для запуска проекта

### 1. Активировать виртуальное окружение

**Windows (PowerShell):**
```powershell
.\venv\Scripts\Activate.ps1
```

**Windows (CMD):**
```cmd
venv\Scripts\activate.bat
```

**Linux/Mac:**
```bash
source venv/bin/activate
```

### 2. Установить зависимости

```bash
pip install -r requirements.txt
```

### 3. Перейти в директорию проекта

```bash
cd blogicum
```

### 4. Применить миграции базы данных

```bash
python manage.py migrate
```

### 5. (Опционально) Создать суперпользователя для админки

```bash
python manage.py createsuperuser
```

Или использовать существующего:
- Логин: `admin`
- Пароль: `admin`

### 6. Запустить сервер разработки

```bash
python manage.py runserver
```

### 7. Открыть в браузере

- Главная страница: http://127.0.0.1:8000/
- Админ-панель: http://127.0.0.1:8000/admin/

## Быстрый запуск (все команды подряд)

**Windows (PowerShell):**
```powershell
.\venv\Scripts\Activate.ps1
pip install -r requirements.txt
cd blogicum
python manage.py migrate
python manage.py runserver
```

**Linux/Mac:**
```bash
source venv/bin/activate
pip install -r requirements.txt
cd blogicum
python manage.py migrate
python manage.py runserver
```

## Остановка сервера

Нажмите `Ctrl+C` в терминале, где запущен сервер.

