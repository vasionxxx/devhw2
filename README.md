# Домашнее задание к занятию «Защита хоста» - Бодарев В.В.

# Задание 1.

---
1.Установите eCryptfs.

2.Добавьте пользователя cryptouser.

3.Зашифруйте домашний каталог пользователя с помощью eCryptfs.

В качестве ответа пришлите снимки экрана домашнего каталога пользователя с исходными и зашифрованными данными.

Установим eCryptfs - sudo apt install ecryptfs-utils.

Создадим нового пользователя cryptouser и зашифруем его домашний каталог - 
sudo ecryptfs-migrate-home -u cryptouser

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/8_1.jpg)

Исходный домашний каталог пользователя

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/8_2.jpg)

Каталог пользователя после шифрования

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/8_3.jpg)

---

# Задание 2.

---

1.Установите поддержку LUKS.

2.Создайте небольшой раздел, например, 100 Мб.

3.Зашифруйте созданный раздел с помощью LUKS.

В качестве ответа пришлите снимки экрана с поэтапным выполнением задания.

Установим LUKS

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/8_4.jpg)

Создадим раздел

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/8_5.jpg)

Зашифруем раздел 

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/8_6.jpg)

Откроем раздел

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/8_7.jpg)

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/8_8.jpg)

Создадим файловую систему 

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/8_9.jpg)

Закроем раздел

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/8_10.jpg)

---


