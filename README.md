# sspyataev_microservices
sspyataev microservices repository


## ДЗ 17 урок
Было сделано:
* Установлены и настроены docker, docker-compose, docker-machine
* Изучены команды docker
* Сделан commit на основе работающего контейнера.
* Создан docker-host в yandex cloud с помощью docker-machine
* Созданы файлы для работы, собран образ, описанный в Dockerfile\
* Проверена работа приложения, запущенного черз docker-machine
* Создан аккаунт на Docker Hub, выложен образ
* Проверена работоспособность образа локально

## ДЗ 18 урок
Было сделано:
* Описаны Dockerfile и собраны docker-образы для приложения
* Изучены основы оптимизации docker-образов
* Запуск приложений через docker run
* Создание network и volume
* Примонтирован volume к контейнеру с БД

## ДЗ 19 урок
Было сделано:
* Рассмотрена работа с типами сетей none и host.
* Создана сеть типа bridge. Запущены контейнеры в созданной сети.
* Рассмотрена работа контейнеров с алиасами сетей.
* Рассмотрен принцип запуска контейнеров через docker-compose
* Создан docker-compose.yml.
* Изменён docker-compose.yml для работы с множеством сетей.
* Параметризированы порт, версия, имя пользователя
* Переменные окружения внесены в файл .env. Для коммита к репу создан файл .env.example
* Базовое имя контейнера, запускаемое через docker-compose можно задать свой, указав внутри каждого сервиса параметр container_name.

## ДЗ 22 урок
Было сделано:
* Рассмотрен prometheus и его базовый конфиг
* Собран собственный образ prometheus со своим конфигом
* Запуск prom добавлен в docker-compose с микросервисами
* Изучена работа с таргетами и джобами, базовые запросы promql
* Рассмотрена схема добавления exporter
* Запушены все микросервисы и prom с конфигом в docker hub
* Ссылка на docker hub repo - https://hub.docker.com/repository/docker/sspyataev/

## ДЗ 21 урок
Было сделано:
* Создан docker-compose для развёртывания gitlab
* Создан проект, запушен репозиторий
* Создан gitlab-ci.yml
* Запущен gitlab runner
* Рассмотрена работа с pipeline gitlab ci
* Рассмторено создание окружений gitlab ci
* Рассмотрена возможность управления этапами pipeline через тэги
* Рассмотрены динамические окружения

## ДЗ 23 урок
Было сделано:
* Рассмотрен и запущен cAdvisor
* Рассмотрена и запущена Grafana
* Добавлен datasource, импортирован дашборб с графана хаб
* Созданы кастомные дашборды для метрик приложения и бизнес метрик
* Использованы функции prometheus rate & histogram_quantile
* Добален и настроен alertmanager
* Создан вебхук для слак
* Ссылка на docker hub repo - https://hub.docker.com/repository/docker/sspyataev/

## ДЗ 24 урок
Было сделано:
* Подготовлены и сконфигурированы сервисы для логирования сервисов
* Развёрнуты elasticsearch, fluentd, kibana
* Рассмотрены запросы и визализация в kibana
* Рассмотрена работа фильтров в fluentd для парсинга логов
* Рассмотрены регулярные выражения и grok паттерны для разбора не структурированных логов
* Сконфигурирован и запущен zipkin для распределённого трейсинга

## ДЗ 28 урок
Было сделано:
* Пройден материал YC Kubernetes the Hart Way
* Рассмотрен принцип ручного разворачивания кластера k8s (одготовка, конфигурирование и т.д.)

## ДЗ 29 урок
Было сделано:
* Установлен minikube
* Рассмотрено управление кластером через kubectl
* Сконфигурированы deployment'ы для приложения
* Сконфигурированы service для связи модулей приложения
* Рассмотрены аддоны minikube
* Создан dev namespace
* Развёрнут кластер kubernetes в YC
* Задеплоено приложение в созданный кластер. Скрин web-интерфейса приложения в PR.

## ДЗ 30 урок
Было сделано:
* Рассмотрены варианты сетевого взаимодействия в k8s
* Создан LoadBalancer, проверена работа приложения
* Создан и сконфигурированы Ingress
* Сконфигурирован TLS и переведено приложение на https
* Создан NetworkPolicy для ограничения доступа к БД
* Рассмотрены и созданы различные варианты хранилищ (Volume, PersistentVolume, PersistentVolumeClaim)
