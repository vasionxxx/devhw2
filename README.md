# Задание 1. СУБД

---

Для решения задач, связанных с управлением данными в крупной строительной компании, можно рассмотреть различные типы систем управления базами данных (СУБД), подходящие для каждой из обозначенных предметных областей.

1.1 Для задач бюджетирования проектов, формирования финансовых аналитических отчетов и прогнозирования рисков лучше всего подойдут реляционные СУБД, такие как PostgreSQL или Microsoft SQL Server. Эти СУБД обеспечивают высокую целостность данных и поддержку сложных запросов, что критично для финансовой аналитики. Они также предлагают механизмы для обеспечения транзакционной целостности (ACID), что важно для работы с финансовыми данными.

1.1* Если хеширование занимает длительное время, можно рассмотреть использование API, таких как HashiCorp Vault или Bcrypt, которые оптимизированы для быстрого хеширования и безопасного хранения данных.

1.2 Для лендингов и CRM-систем лучше использовать NoSQL СУБД, такие как MongoDB или Firebase. Эти системы обеспечивают гибкость в структуре данных и высокую скорость обработки запросов, что критично для работы с большим количеством лидов и динамическими данными.

1.2* Да, эту задачу можно решить одной СУБД. Например, MongoDB может быть использована как для лендингов, так и для CRM, благодаря своей гибкости и возможностям масштабирования.

1.3 Для создания базы данных по корпоративным нормам и обучающим материалам подойдет реляционная СУБД, такая как SQLite или MySQL. Эти СУБД имеют простую и понятную структуру, что облегчает создание и поддержку базы данных.

1.3* Да, можно использовать уже существующую реляционную СУБД из предыдущих задач. Например, если используется PostgreSQL для бюджетирования, можно создать отдельные таблицы для хранения корпоративных норм и правил в той же базе данных.

1.4 Для задач логистики, требующих быстрого формирования маршрутов и работы со связями, лучше всего подойдет графовая СУБД, такая как Neo4j. Она позволяет эффективно моделировать и обрабатывать сложные взаимосвязи между объектами, что критично для задач маршрутизации.

1.4* Да, можно подключить отдел закупок к той же СУБД, если используется графовая модель, так как это позволит эффективно управлять взаимосвязями между поставщиками и логистическими процессами.

1.5 Возможно использовать одну СУБД для всех перечисленных задач, однако это будет зависеть от специфики реализации. Например, PostgreSQL может быть универсальным решением, так как она поддерживает как реляционные, так и некоторые NoSQL возможности. Однако для специфических задач, таких как маршрутизация, может потребоваться использование специализированной графовой СУБД.

---

# Задание 2. Транзакции

---

2.1 Для успешного пополнения баланса счёта телефона пользователю необходимо выполнить следующие шаги:

1.	Выбор способа пополнения: Пользователь выбирает способ пополнения счёта, например, через мобильное приложение, банкомат или сайт оператора связи.
   
2.	Ввод данных: Пользователь вводит номер телефона, который необходимо пополнить, и сумму пополнения.
   
3.	Выбор способа оплаты: Пользователь выбирает способ оплаты, например, банковскую карту, электронный кошелёк или наличные.

4.	Подтверждение транзакции: Пользователь подтверждает транзакцию, проверяя введенные данные и согласившись с условиями.
	
5.	Обработка платежа: Система обрабатывает платеж, проверяя наличие средств на счёте пользователя и выполняя необходимые операции с платёжной системой.
	
6.	Уведомление о завершении: После успешного завершения транзакции пользователь получает уведомление о пополнении баланса, а средства зачисляются на счёт телефона.

2.1* Если пополнение счёта телефона происходит через автоплатёж, процесс будет следующим:
   	
1.	Настройка автоплатежа: Пользователь в личном кабинете оператора связи настраивает автоплатёж, указывая номер телефона, сумму и периодичность списания.
   
2.	Привязка банковской карты: Пользователь привязывает свою банковскую карту к автоплатежу, обеспечивая доступ к средствам для автоматического списания.
   
3.	Подтверждение настроек: Пользователь подтверждает настройки автоплатежа, проверяя все введенные данные.
   
4.	Автоматическое списание: В установленный день происходит автоматическое списание средств с банковской карты пользователя.
   
5.	Обработка платежа: Система обрабатывает платеж и проверяет наличие средств на счёте.
    
6.	Уведомление о пополнении: Пользователь получает уведомление о том, что баланс его телефона успешно пополнен.
	
---

# Задание 3. SQL vs NoSQL

---

3.1 Преимущества SQL-систем по отношению к NoSQL:

1.	Строгая структура данных: SQL-системы используют фиксированную схему данных, что обеспечивает высокую целостность и согласованность данных. Это особенно важно для приложений, где требуется строгий контроль за данными и их структурой.
   
2.	Поддержка транзакций: SQL-системы обеспечивают соответствие требованиям ACID (атомарность, согласованность, изолированность, долговечность), что гарантирует надежность выполнения транзакций и защиту данных от потерь.
   
3.	Сложные запросы: SQL предоставляет мощный язык запросов, позволяющий выполнять сложные выборки и манипуляции с данными. Это делает SQL-системы более подходящими для аналитических задач и отчетности.
	
4.	Безопасность данных: SQL-системы предлагают продвинутые механизмы управления доступом, позволяя настраивать права пользователей и обеспечивать безопасность данных на уровне строк и столбцов.
   
5.	Широкая поддержка и экосистема: SQL-системы имеют долгую историю и широкую поддержку со стороны разработчиков, что обеспечивает наличие большого количества инструментов, библиотек и документации для работы с ними.
    
3.1* Преимущества NewSQL систем
   	
NewSQL системы предлагают следующие преимущества по сравнению с традиционными SQL и NoSQL:

1.	Высокая производительность: NewSQL системы обеспечивают производительность, сопоставимую с NoSQL, благодаря использованию современных архитектур и оптимизированных алгоритмов обработки данных, что позволяет обрабатывать большие объемы транзакций.
   
2.	Поддержка ACID: В отличие от многих NoSQL систем, NewSQL сохраняют требования ACID, что делает их подходящими для приложений, где важна надежность и согласованность данных.
   
3.	Гибкость масштабирования: NewSQL системы предлагают горизонтальное масштабирование, что позволяет легко добавлять новые узлы в кластер и увеличивать производительность без значительных затрат на инфраструктуру.
   
4.	Сохранение реляционной модели: NewSQL системы поддерживают реляционную модель данных и SQL, что упрощает миграцию с традиционных SQL-систем и использование существующих навыков разработчиков.
   
5.	Интеграция с облачными решениями: Многие NewSQL системы оптимизированы для работы в облачных средах, что позволяет эффективно использовать ресурсы и повышать доступность приложений.
   
---

# Задание 4. Кластеры

---

Для решения задачи, связанной с большими данными и распределенными вычислениями, необходимо выбрать тип СУБД и модель распределенных вычислений, которые будут наиболее эффективными и масштабируемыми.
При выборе типа СУБД ключевым критерием будет способность системы эффективно обрабатывать большие объемы неструктурированных данных и поддерживать горизонтальное масштабирование. Исходя из этого, наиболее подходящим вариантом будут NoSQL СУБД, такие как:

•	Apache Hadoop - распределенная платформа для хранения и обработки больших данных, использующая модель MapReduce для распараллеливания вычислений.

•	Apache Spark - платформа для распределенных вычислений, обеспечивающая высокую производительность обработки данных с использованием оперативной памяти.

•	MongoDB - документоориентированная NoSQL СУБД, позволяющая хранить и обрабатывать большие объемы неструктурированных данных.

Для распределения вычислений на 1000 машин наиболее подходящей будет модель MapReduce, реализованная в таких системах, как Apache Hadoop и Apache Spark.MapReduce разбивает задачу на множество независимых подзадач, которые могут выполняться параллельно на разных машинах. Это позволяет эффективно обрабатывать большие объемы данных, используя вычислительные ресурсы множества узлов.

Преимущества MapReduce:

•	Высокая масштабируемость за счет распределения вычислений на множество машин.
•	Отказоустойчивость, так как система автоматически обрабатывает сбои отдельных узлов.
•	Простота программирования, так как разработчики могут сфокусироваться на логике обработки данных, не заботясь о деталях распределения вычислений.

Таким образом, для решения задачи с большими данными и распределенными вычислениями на 1000 машин, наиболее подходящим вариантом будет использование NoSQL СУБД, таких как Apache Hadoop или Apache Spark, в сочетании с моделью MapReduce для распределения вычислений. Это обеспечит высокую производительность, масштабируемость и отказоустойчивость системы.

---
