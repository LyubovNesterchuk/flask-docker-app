Створення проєкту

1.Створити проєкт у GitHub Codespaces.
Створити файли: app.py, requirements.txt, Dockerfile

2. Встановлення Flask
pip install flask

3. Збереження залежностей
pip freeze > requirements.txt

4. Очищення requirements.txt (залишити тільки: Flask==3.1.3)

5. Запуск застосунку
python app.py

6. Перевірка роботи (відкрити у браузері: http://localhost:5000)

7. Створення Docker image
docker build -t myname/flask-docker .

8. Запуск контейнера
docker run -p 5000:5000 myname/flask-docker


Як закінчити роботу?

1. Зупини сервер Flask (якщо він запущений, Ctrl + C  зупинить python app.py)

2. Закрий Docker контейнер (якщо запущений, то подивитись активні контейнери: docker ps,
щоб побачити всі контейнери (навіть зупинені): docker ps -a )
docker stop <container_id>

3. Збережи всі файли, закоміть і запуш у GitHub 
У терміналі:
git add .
git commit -m "..."
git push

5. Закрити Codespaces
у браузері:  ≡ (меню) → Codespaces → Stop Codespace
або:
зайди на GitHub Codespaces → Your codespaces натисни Stop
