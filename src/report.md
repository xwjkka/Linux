# Операционные системы UNIX/Linux (Базовый).

Установка и обновления системы Linux. Основы администрирования.

## Part 1. Установка ОС

Ubuntu 20.04 Server LTS** без графического интерфейса
- ![Ubuntu 20.04 Server LTS** без графического интерфейса](imgs/1.png)

## Part 2. Создание пользователя

Вызов команды для создания пользователя
- ![Вызов команды для создания пользователя](imgs/2.png)
- ![Вызов команды для создания пользователя](imgs/3.png)

## Part 3. Настройка сети ОС

Меням hostname, timezone. 
- ![hostname](imgs/4.png)
- ![timezone](imgs/5.png)
- ![ip addresses](imgs/6.1.png)
- lo - внутреняя сеть, en... - внешняя
- ![ip addresses DHCP](imgs/7.png)
- Dynamic Host Configuration Protocol — протокол динамической настройки узла  

внешний ip-адрес шлюза
- ![ip addresses DHCP](imgs/8.png)

внутренний IP-адрес шлюза
- ![внутренний IP-адрес шлюза](imgs/9.png)

Задаем статические настройки ip, gw, dns
- ![изменение файлика ...](imgs/10.png)
- ![сохранение изменений](imgs/11.png)
- ![обновляем виртуальную машину](imgs/15.png)
- ![после обновления изменения сохранились](imgs/14.png)

0 loss - значит все правильно!
- ![ping 1.1.1.1](imgs/12.png)
- ![ping ya.ru](imgs/13.png)

## Part 4. Обновление ОС

- ![ос обновлена](imgs/16.png)

## Part 5. Использование команды **sudo**

- Главное назначение sudo — это выполнить команду от имени другого пользователя, обычно от root.
- ![+ права пользователю](imgs/17.png)
- ![меняем hostname](imgs/58.png)

## Part 6. Установка и настройка службы времени

- ![синхронизация включена](imgs/18.png)
- ![текущее время](imgs/19.png)

## Part 7. Установка и использование текстовых редакторов

- ![vim](imgs/20.png)
- esc :wq
- ![nano](imgs/21.png)
- ^С y ^M
- ![joe](imgs/22.png)
- ^KX

##### 2

- ![vim](imgs/23.png)
- esc :q!
- ![nano](imgs/24.png)
- ^С n
- ![joe](imgs/25.png)
- ^C y

##### 3

- ![vim](imgs/26.png)
- /что ищем
- ![vim](imgs/27.png)
- :s/что меняем/замена

- ![nano](imgs/28.png)
- ^W что ищем
- ![nano](imgs/29.png)
- ^R замена y
- ![joe](imgs/30.png)
- ^KF что ищем entr
- ![joe](imgs/31.png)
- ^KF что заменяем entr R замена

## Part 8. Установка и базовая настройка сервиса **SSHD**

-  sudo apt install openssh-server (устанавливаем службу)
-  ![открываем файл конфигурации с помощью vim](imgs/32.png)
-  ![меняем порт на Port 2022](imgs/33.png)
-  ![ps aux - запущенные процессы, grep - выбрать с портом 2022](imgs/34.png)

## Part 9. Установка и использование утилит **top**, **htop**

- ![top](imgs/35.png)
    - uptime 5:39
    - количество авторизованных пользователей 1 user
    - общую загрузку системы 0.00
    - общее количество процессов 108
    - cpu 0.0 
    - загрузку памяти 976.9
    - pid процесса занимающего больше всего памяти 1 root
    - pid процесса, занимающего больше всего процессорного времени 1 root

fdisk
- ![sort PERCENT_CPU](imgs/37.png)
- ![sort PERCENT_MEM](imgs/39.png)
- ![sort TIME](imgs/40.png)
- ![filter sshd](imgs/41.png)
- ![search syslog](imgs/42.png)
- ![+ hostname, clock, uptime](imgs/43.png)

## Part 10. Использование утилиты **fdisk**

- ![fdisk](imgs/44.png)

## Part 11. Использование утилиты **df**

- ![df /](imgs/45.png)
- ![df -Th /](imgs/46.png)

## Part 12. Использование утилиты **du**

- ![du](imgs/54.png)

- ![/home](imgs/55.png)
- ![/var](imgs/56.png)
- ![/var/log](imgs/57.png)

## Part 13. Установка и использование утилиты **ncdu**

- ![home](imgs/47.png)
- ![var](imgs/48.png)
- ![var/log](imgs/49.png)

## Part 14. Работа с системными журналами

- ![последний logtime](imgs/52.png)
- ![новый](imgs/52.png)

## Part 15. Использование планировщика заданий **CRON**

- ![cron](imgs/51.png)
- ![cron](imgs/50.png)
- ![cron](imgs/53.png)
