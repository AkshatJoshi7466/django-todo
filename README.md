# django-todo
A simple todo app built with django

![todo App](https://raw.githubusercontent.com/shreys7/django-todo/develop/todoApp/staticfiles/todoApp.png)
### Setup
To get this repository, run the following command inside your git enabled terminal
```bash
$ git clone https://github.com/shreys7/django-todo.git
```
You will need django to be installed in you computer to run this app. Head over to https://www.djangoproject.com/download/ for the download guide

Once you have downloaded django, go to todoApp directory and run the following command



```bash
$ pip insatll django
$ python manage.py makemigrations
```

This will create all the migrations file (database migrations) required to run this App.

Now, to apply this migrations run the following command
```bash
$ python manage.py migrate
```

That was pretty simple, right? Now let's make the App live. We just need to start the server now and then we will start using our simple todo App. Start the server by following command

```bash
$ python manage.py runserver
```

Once the server is hosted, head over to http://127.0.0.1:8000/todos for the App.

Host on server  
```bash
$ python manage.py runserver 0.0.0.0:3000

or run in background

$ nohup python manage.py runserver 0.0.0.0:3000 & 

### NOTE setting.py ALLOWED_HOSTS = [] // 'IP or *'
```
Deploy on with Docker file

create docker file

```bash
$ sudo docker build . -t django-app

$ sudo docker run -p 3000:3000 < container_id >

$ sudo docker run -d -p 3000:3000 <container_id > # with deamon and background run 

```


