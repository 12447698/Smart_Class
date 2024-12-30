# 🔧 Smart Class: Инструкция по запуску

Следуйте этой инструкции для настройки и запуска проекта **Smart Class**. Все команды выполняются в терминале.  
**Важно:** Убедитесь, что у вас установлены `Python` и `pip`.

---

## 💻 Запуск проекта

### 1️⃣ Клонируйте проект:
```bash
git clone https://github.com/124476/SmartClass
```

### 2️⃣ Перейдите в папку проекта:
```bash
cd SmartClass
```

### 3️⃣ Создайте и активируйте виртуальное окружение:
#### Для Windows:
```bash
python -m venv venv
venv\Scripts\activate
```
#### Для macOS/Linux:
```bash
python3 -m venv venv
source venv/bin/activate
```

### 4️⃣ Установите зависимости:
```bash
pip install -r requirements.txt
```

### 5️⃣ Перейдите в папку с `manage.py`:
```bash
cd smart_class
```

### 6️⃣ Примените миграции:
```bash
python manage.py migrate
```

### 7️⃣ Запустите сервер:
```bash
python manage.py runserver
```

### 8️⃣ Откройте сайт:
Перейдите по адресу:  
[http://127.0.0.1:8000/](http://127.0.0.1:8000/)

> **Важно:** Не закрывайте терминал, пока сервер работает.

---

## ⚠ Возможные ошибки запуска

### 🛠 Ошибка при активации `venv\Scripts\activate` (Windows):
Решение:
1. Откройте PowerShell **от имени администратора**.
2. Выполните команду:
   ```bash
   Set-ExecutionPolicy RemoteSigned
   ```
3. Подтвердите, введя `A`.
4. Повторите активацию виртуального окружения.

### 🛠 Ошибка при загрузке `requirements.txt`:
Если на вашем устройстве установлено несколько версий Python, укажите путь к конкретной версии.  

#### Пример для Windows:
```bash
C:\path\to\python3.8\python.exe -m venv venv
```

#### Пример для macOS/Linux:
```bash
python3.8 -m venv venv
```

---

💡 **Совет:** Если у вас возникнут вопросы, создайте Issue в репозитории GitHub.
