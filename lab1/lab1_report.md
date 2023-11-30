University: [ITMO University](https://itmo.ru/ru/) <br>
Faculty: [FICT](https://fict.itmo.ru) <br>
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)
Year: 2023/2024 <br>
Group: K4110c <br>
Author: Akhmetzhanov Renat Ruslanovich <br>
Lab: Lab1 <br>
Date of create: 15.10.2023 <br>
Date of finished:  <br>


1.Устанавливаем и запускаем minikube.
![Alt text](images/image.png)

2.Скачиваем контейнер vault 
![Alt text](images/image-1.png)

3.Создаём yaml манифест для создания деплоймента.
![Alt text](images/image-2.png)

4.Разворачиваем его в кластере.
![Alt text](images/image-3.png)

5. Деплой сервиса и проброс порта
![Alt text](images/image-4.png)

6.Открываем vault в браузере по заданному порту
![Alt text](images/image-5.png)

7.Для получения токена для входа в vault открываем логи пода. Смотрим логи через графический интерфейс запуском minikube dashboard
![Alt text](images/image-6.png)

8.Авторизация при помощи полученного токена.
![Alt text](images/image-7.png)

Ответы на вопросы:

1. Было развернуто приложение для хранения секретов vault в кубере. Для этого был развернут один деплоймент с двумя подами и 1 сервис для подключения к нему.

2. Токен для входа в vault хранится в логах пода.

Схема

![Alt text](images/scheme.png)