# Домашнее задание к занятию «Disaster recovery и Keepalived» - BodarevVV
# Задание №1.
# Настраиваем отслеживание состояния интерфейсов. 

![alt text](https://github.com/vasionxxx/devhw2/blob/main/CICD/q11.png)


# Отсоединяем кабель и запускаем ping..

![alt text](https://github.com/vasionxxx/devhw2/blob/main/CICD/q12.jpg)

# Задание №2.
# Запускаем 2 виртуальные машины, устанавливаем и настраиваем сервер keepalived. Запускаем веб-сервер на виртуальных машинах с помощью команды - python3 -m http.server 8080 &. Пишем Bash-скрипт, который будет проверять доступность порта данного веб-сервера и существование файла index.html.

[Bash-скрипт](https://github.com/vasionxxx/devhw2/blob/main/CICD/check_webserver.sh.txt)

# Настраиваем Keepalived

[Keepalived](https://github.com/vasionxxx/devhw2/blob/main/CICD/keepalived.conf.txt)

# Выключаем первую виртуальную машину и проверяем статус keeplived и видим, что вторая виртуальная машина стала “MASTER STATE” и ip адрес 172.24.77.77 указанный в keepalived.conf, если включить первую виртуальную машину то вторая станет “BACKUP STATE”.

![alt text](https://github.com/vasionxxx/devhw2/blob/main/CICD/q22.jpg)
![alt text](https://github.com/vasionxxx/devhw2/blob/main/CICD/q21.jpg)
