University: [ITMO University](https://itmo.ru/ru/)

Course: [IP-telephony](https://itmo-ict-faculty.github.io/ip-telephony/)

Year: 2024/2025

Group: K34212

Author: Petrov Dmitriy Konstantinovich

Lab: Lab2

Date of create: 25.04.2025

Date of finished: 25.04.2025


## Отчет по лабораторной работе №2:
### "Конфигурация voip в среде Сisco packet tracer"

#### 1. Цель:
Изучить построение сети IP-телефонии с помощью маршрутизатора Cisco 2811, коммутатора Cisco catalyst 3560 и IP телефонов Cisco 7960.

#### 2. Ход работы:

#### Часть 1

Схема 1:

![img.png](img.png)

Сначала был настроен роутер. Было изменено имя, далее был отключен синтаксис ввода слов от DNS серверов,
затем был выдан ip адрес интерфейсу fa0/0 и настроен DHCP пул для голосовой сети.

![img_1.png](img_1.png)

После был настроен свитч:

![img_2.png](img_2.png)

Далее были настроены номера телефонов:

![img_3.png](img_3.png)

Попытки звонков:

![img_4.png](img_4.png)

![img_5.png](img_5.png)

![img_6.png](img_6.png)

#### Часть 2

Была собрана схема, согласно заданию

![img_7.png](img_7.png)

Были созданы вланы для звонков и данных, после чего порт fa0/1 переведен в trunk режим, а порты fa0/2-4 в access режим.

![img_8.png](img_8.png) 

Далее были настроены два DHCP сервера

![img_9.png](img_9.png)

Далее были созданы логические подинтерфейсы с инкапсуляцией Dot1Q, а также настроен телефонный сервис и выданы номера для телефонов

![img_10.png](img_10.png)

Далее были разданы ip адреса для компьютеров посредством DHCP

![img_11.png](img_11.png)

Проверим связность

![img_12.png](img_12.png)

Совершим звонок

![img_13.png](img_13.png)