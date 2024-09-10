# Домашнее задание к занятию "Кеширование Redis/memcached"

# Задание 1. Кеширование

---

Вот несколько примеров проблем, которые можно решить с помощью кеширования:
Повышение производительности
Кеширование позволяет значительно ускорить доступ к часто используемым данным, так как они хранятся в памяти, а не запрашиваются из базы данных или другого медленного источника. Это особенно актуально для приложений, работающих в режиме реального времени, где каждая миллисекунда на счету.
Снижение нагрузки на источник данных
Кеширование уменьшает количество запросов к базе данных, внешним API и другим медленным источникам данных. Это помогает избежать перегрузки источника при пиковых нагрузках и обеспечивает стабильную работу системы.
Решение проблемы "холодного старта"
При запуске приложения или после сброса кеша, первые запросы будут промахами, так как данные еще не загружены в кеш. Чтобы избежать этой проблемы, можно использовать техники "прогревания" кеша при старте приложением, загружая в него наиболее востребованные данные.
Кеширование ошибок
Если приложение часто получает одни и те же ошибки при попытке доступа к данным, их можно кешировать. Это позволит быстрее реагировать на ошибки и снизит нагрузку на источник данных.
Согласованность данных между серверами
В распределенных системах кеш в памяти на разных серверах может содержать несогласованные данные. Использование внешнего централизованного кеша помогает решить эту проблему.Таким образом, кеширование является мощным инструментом для повышения производительности, масштабируемости и надежности приложений. Однако его нужно правильно настраивать и учитывать возможные проблемы, чтобы извлечь максимальную пользу.

---

# Задание 2. Memcached

---
Установим memcached и проверим что он запущен. 
![image alt](https://github.com/vasionxxx/devhw2/blob/main/CICD/31.jpg)
	
---

# Задание 3. SQL vs NoSQL

---

   
---

# Задание 4. Кластеры

---

---
