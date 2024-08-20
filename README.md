# Домашнее задание к занятию «Кластеризация и балансировка нагрузки» - BodarevVV
# Задание №1.
# Запускаем два simple python сервера. Создаем 2 файла srv1.py и srv2.py. Скриншоты содержимого файлов srv1.py и srv2.py:

![alt text](https://github.com/vasionxxx/devhw2/blob/main/CICD/3_1.jpg)
![alt text](https://github.com/vasionxxx/devhw2/blob/main/CICD/3_2.jpg)

# Запускаем сервер с помощью команд python3 srv1.py и python3 srv2.py. Проверяем работу сервера зайдя на него.

![alt text](https://github.com/vasionxxx/devhw2/blob/main/CICD/3_3.jpg)

# Устанавливаем HAProxy с помощью команды - sudo apt-get install haproxy. 
Настраиваем балансировку. 
Скриншот файла haproxy.cfg:
![alt text](https://github.com/vasionxxx/devhw2/blob/main/CICD/3_4.jpg)

# Перезапускаем HAProxy - sudo systemctl restart haproxy и проверяем работу. Видно, что при обновлении страницы нас перенаправляет на разные сервера.

![alt text](https://github.com/vasionxxx/devhw2/blob/main/CICD/3_5.jpg)
![alt text](https://github.com/vasionxxx/devhw2/blob/main/CICD/3_6.jpg)

# Файл HAProxy https://github.com/vasionxxx/devhw2/blob/main/CICD/haproxy1.txt

# Задание №2.
# Запускаем три simple python сервера по аналогии с первым заданием. Настраиваем балансировку Weighted Round Robin на 7 уровне, чтобы первый сервер имел вес 2, второй - 3, а третий – 4. Скриншот настроек:

![alt text](https://github.com/vasionxxx/devhw2/blob/main/CICD/3_7.jpg)

# Проверим работу. Видно что запросы перенаправляются. 

![alt text](https://github.com/vasionxxx/devhw2/blob/main/CICD/3_8.jpg)

# Если же обратится без указания хоста, появится ошибка

![alt text](https://github.com/vasionxxx/devhw2/blob/main/CICD/3_9.jpg)

# Файл HAProxy https://github.com/vasionxxx/devhw2/blob/main/CICD/haproxy2.txt
