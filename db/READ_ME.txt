1. Переходим в папку с Dockerfile командной "cd <адрес_папки "db">";
2. Для сборки docker-образа вводим команду "docker build -t test_image:latest ."
3. Запускаем контейнер командой "docker run -d -p 5432:5432 --name <имя_контейнера> test_image:latest 
4. Для сохранения изменений в контейнере дополняем команду из пункта 3 следующим содержимым "-v /data:/var/lib/postgresql/data postgres"
 