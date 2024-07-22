# Домашнее задание к занятию «Система мониторинга Zabbix» - BodarevVV
№ Задание №1
# Авторизация в админке
![alt text](https://github.com/vasionxxx/devhw2/blob/main/gitlab/11.jpg)

# Команды
```
apt install postgresql 
wget https://repo.zabbix.com/zabbix/6.0/ubuntu/pool/main/z/zabbix-release/zabbix-release_6.0-4+ubuntu22.04_all.deb
dpkg -i zabbix-release_6.0-4+ubuntu22.04_all.deb
apt update
apt install zabbix-server-pgsql zabbix-frontend-php php8.1-pgsql zabbix-apache-conf zabbix-sql-scripts zabbix-agent
su – postgres -c ‘psql –command “CREATE USER Zabbix WITH PASSWORD ‘\’123456789\’’;”’
su – postgres -c ‘psql –command “CREATE DATABASE zabbix OWNER zabbix;”’ 
zcat /usr/share/zabbix-sql-scripts/postgresql/server.sql.gz | sudo -u zabbix psql Zabbix
Меняем 
systemctl restart zabbix-server zabbix-agent apache2
systemctl enable zabbix-server zabbix-agent apache2

```

# № Задание №2
# Подключенные хосты
![alt text](https://github.com/vasionxxx/devhw2/blob/main/gitlab/21.jpg)

# Лог Zabbix agent 
![alt text](https://github.com/vasionxxx/devhw2/blob/main/gitlab/22.jpg)

# Поступающие данные от агентов
![alt text](https://github.com/vasionxxx/devhw2/blob/main/gitlab/23.jpg)

# Команды
```
wget https://repo.zabbix.com/zabbix/6.0/ubuntu/pool/main/z/zabbix-release/zabbix-release_6.0-4+ubuntu22.04_all.deb
dpkg -i zabbix-release_6.0-4+ubuntu22.04_all.deb
apt update
apt install zabbix-agent
systemctl restart zabbix-agent
systemctl enable zabbix-agent

```
