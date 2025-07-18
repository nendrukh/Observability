## GAP-1 ##

### Описание сделанного задания
Задание сделал с помощью докер контейнеров из подготовленных образов. Есть prometheus, CMS (WordPress), MySQL, MySQL-exporter и blackbox-exporter, который проверяет CMS.

Использовал следующие образы:
* mysql:8.4
* prom/prometheus:v3.4.2
* prom/mysqld-exporter:v0.17.2
* wordpress:php8.4-apache
* prom/blackbox-exporter:v0.27.0

Для запуска нужно ввести команду в директории GAP-1:
```shell
docker-compose up --build
```

WordPress находится на 8080 порту: http://localhost:8080/

Prometheus находится на 9090 порту: http://localhost:9090/
