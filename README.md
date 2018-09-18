db-docker
---------

Копия MySQL  баз данных доступных с сервера works.rg.ru.
по состояннию на 2018.09.04.


Используется для локальной разработки приложений в докерах.
Перед запуском какого-либо приложения необходимо запустить это приложение.


**Доступные базы данных:** 
comments, d2, front, jurist, mysql, outer, performance_schema, subs, subsmag, works

----------

#### Требуемое ПО
На компьютере разработчика должно быть установлены:
* [Git](https://git-scm.com/downloads)
* [Docker](https://docs.docker.com/engine/installation/)
* [Docker Compose](https://docs.docker.com/compose/install/)


--------------------------

**Запуск**:

```sh
docker-compose up -d
```

> На старт базы данных может потребоваться время. Состояние контейнеров в реальном времени можно посмотреть командой:
```sh
sudo docker-compose logs -f 
```
> Прервать просмотр логов `Ctrl-C`.



Временный останов:
```sh
docker-compose stop
```


Пуск остановленного приложения:
```sh
docker-compose start
```


Удаление с компьютера
```sh
docker-compose down
```


Просмотр лога
```sh
docker-compose logs -f
```


Просмотр базы данных в phpmyadmin:
http://localhost:8082
login:root
password:root




Локальный MySQL порт: 8989

 




