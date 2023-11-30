University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FICT](https://fict.itmo.ru)
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)
Year: 2023/2024
Group: K4110c
Author: Akhmetzhanov Renat Ruslanovich
Lab: Lab3
Date of create: 28.11.2023
Date of finished: 

1.Запускаем minikube с подключенным плагином CNI=calico, режимом работы Multi-Node Clusters и разворачиваем 2 ноды 
![Alt text](images/image.png)

2.Проверяем количество нод и подов calico
![Alt text](images/image-1.png)

3.Помечаем ноды по географическому положению
![Alt text](images/image-9.png)

4.Создание файла манифеста для назначения пула IP узлам на основе их меток.
![Alt text](images/image-2.png)

5.Удаляем дефолтный Ippools перед созданием своих и создаем свои
![Alt text](images/image-10.png)

6.Создаем деплоймент приложения
![Alt text](images/image-11.png)

7.Проверяем, какие ip адреса были назначены. Адреса из тех ippool которые мы создавали, следовательно, всё настроено верно.
![Alt text](images/image-12.png)

8.Создаем сервис и прокидываем 3000 порт
![Alt text](images/image-7.png)

9.Заходим на сайт и видим, что все настроено верно и ip контейнера назначен верно. Container name и Container IP могут меняться, в зависимости от того, на какой под попал запрос.
![Alt text](images/image-6.png)

10.Заходим в один из подов и пингуем соседний 
![Alt text](images/image-8.png)

11. Схема
![Alt text](images/image-13.png)

