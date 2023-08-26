# infra_sprint1
#Описание

	Kittygram — социальная сеть для обмена фотографиями любимых питомцев.
	Это полностью рабочий проект, который состоит из бэкенд-приложения на Django и фронтенд-приложения на React.

#Подключение к удалённому серверу по SSH-ключу

	ssh -i путь_до_SSH_ключа/название_файла_с_SSH_ключом_без_расширения login@ip

#Клонирование проекта с GitHub на сервер

	git clone git@github.com:ваш_аккаунт/название_репозитория.git

#Установите зависимости из файла requirements.txt:
	
	1)cd название_проекта/backend/
	2)python3 -m venv venv
	3)source venv/bin/activate
	4)pip install -r requirements.txt

#Выполните миграции и создайте суперюзера из директории с файлом manage.py:

	1)python3 manage.py migrate
	2)python3 manage.py createsuperuser

#Установка и настройка WSGI-сервера Gunicorn

	1)Подключитесь к удалённому серверу, активируйте виртуальное окружение бэкенд-приложения и установите пакет gunicorn:
		pip install gunicorn==20.1.0

#Установка и настройка веб- и прокси-сервера Nginx

	1)sudo apt install nginx -y
	2)sudo systemctl start nginx

#Автор проекта:
	
	Владислав Ермаков, https://github.com/Vladislav199912
