# Домашнее задание к занятию «Работа с данными (DDL/DML)» - Бодарев В.В.

# Задание 1.

---

1.1.	Установим MySQL

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/4_1.jpg)

---

---

1.2.	Создадим учётную запись sys_temp

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/4_2.jpg)

---

---

1.3.	Выполним запрос на получение списка пользователей в базе данных

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/4_3.jpg)

---

---

1.4.	Дадим все права для пользователя sys_temp.

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/4_4.jpg)

---

---

1.5.	Выполним запрос на получение списка прав для пользователя sys_temp.

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/4_5.jpg)

---

---

1.6.	Переподключимся к базе данных от имени sys_temp.

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/4_6.jpg)

Для смены типа аутентификации с sha2 используем запрос:
ALTER USER 'sys_test'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/4_7.jpg)

---

---

1.7.	По ссылке https://downloads.mysql.com/docs/sakila-db.zip скачиваем дамп базы данных.

---

---

1.8.	Восстановим дамп в базу данных.

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/4_8.jpg)

---

---

1.9.	Получаем список всех таблиц в базе данных.

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/4_9.jpg)

# Задание 2.

---

![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/4_10.jpg)

---


