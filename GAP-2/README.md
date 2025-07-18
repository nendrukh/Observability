## GAP-2 ##

### Описание сделанного задания
Задание сделал из образов из предыдущего задания. Добавил хранилище метрик Victoria Metrics.
Во время записи метрик в хранилище Prometheus добавляет лейбл site: prod.
И при запуске Victoria Metrics прокидывается команда -retentionPeriod=2w

Использовал следующие образы:
* mysql:8.4
* prom/prometheus:v3.4.2
* prom/mysqld-exporter:v0.17.2
* wordpress:php8.4-apache
* prom/blackbox-exporter:v0.27.0
* victoriametrics/victoria-metrics:v1.121.0

Для запуска нужно ввести команду в директории GAP-2:
```shell
docker-compose up --build
```

WordPress находится на 8080 порту: http://localhost:8080/

Prometheus находится на 9090 порту: http://localhost:9090/

Victoria Metrics находится на 8428 порту: http://localhost:8428/vmui
