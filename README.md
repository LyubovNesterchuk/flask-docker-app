# flask-docker-app


# ✔ Послідовність дій

## 1. Створення проєкту
Створити проєкт у GitHub Codespaces.

Створити файли:
- `app.py`
- `requirements.txt`
- `Dockerfile`

---

## 2. Встановлення Flask
```bash
pip install flask
3. Збереження залежностей
pip freeze > requirements.txt
4. Очищення requirements.txt

Залишити тільки:

Flask==3.1.3
5. Запуск застосунку
python app.py
6. Перевірка роботи

Відкрити у браузері:

http://localhost:5000
7. Створення Docker image
docker build -t myname/flask-docker .
8. Запуск контейнера
docker run -p 5000:5000 myname/flask-docker

1. Зупини сервер Flask (якщо він запущений)

У терміналі натисни:

Ctrl + C

👉 це зупинить python app.py

🟢 2. Закрий Docker контейнер (якщо запускала)

Подивись активні контейнери:

docker ps

Зупинка:

docker stop <container_id>

(або просто закрий вкладку terminal — але краще stop)
Щоб побачити ВСІ контейнери (навіть зупинені):

docker ps -a

🟢 3. Збережи всі файли

🟢 4. Закоміть і запуш у GitHub (ВАЖЛИВО для здачі)

У терміналі:

git add .
git commit -m "Finish Flask Docker project"
git push
🟢 5. Закрити Codespaces

У браузері:

👉 натисни у верхньому лівому куті:

≡ (меню) → Codespaces → Stop Codespace

або:

зайди на GitHub
Codespaces → Your codespaces
натисни Stop