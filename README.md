# Домашнее задание к занятию 11.1. «Базы данных, их типы» - Пугач Евгений.


---

### Задание 1. СУБД

##Ответ:

1.1 Подойдёт реляционная СУБД.

1.2 Для CRM однозначно следует использовать реляционную СУБД, а для лендингов можно использовать объектно-ориентированную или реляционную СУБД.

1.3 Подойдет документо-ориентированная, либо реляционная СУБД.

1.4 Скорее подойдет графовая СУБД, но можно использовать и реляционную СУБД.

1.5 Да, во всех вышеперечисленных случаях можно использовать только реляционную СУБД, с определенными доработками.


---

### Задание 2. Транзакции

##Ответ:

2.1 Как действуют люди старшего поколения:

1. Пользователь идет в салон сотового оператора, дожидается своей очереди;
2. Называет сотруднику салона номер телефона (передает на листе бумаги), счет которого хочет пополнить, передает ему наличные;
3. Сотрудник переспрашивает номер для исключения ошибки, совершает неведомые действия перед монитором с использованием клавиатуры;
4. Распечатывает и передает пользователю чек об оказании услуги пополнения счета мобильного телефона;
5. Если при вводе номера сотрудником не произошло ошибки, то через некоторое время на названный номер приходит уведомление о пополнении баланса. Профит!

А если серьезно, то:

1. Пользователь отправляет запрос в банк об авторизации (через приложение, либо онлайн, либо лично, посредством предъявления паспорта);
2. При успешной верификации пользователь получает доступ к своему счету;
3. Пользователь формирует поручение банку на перевод суммы на счет мобильного телефона;
4. Банк проверяет наличие указанной суммы на счете пользователя, в случае положительного результата уточняет, какой банк обслуживает счет мобильного оператора, баланс номера которого желает пополнить пользователь, осуществляет перевод и выдает пользователю документ, подтверждающий проведение операции;
5. Банк, обслуживающий мобильного оператора, уведомляет его о поступлении средств на счет;
6. Мобильный оператор проверяет наличие номера телефона, указанного при переводе, в базе обслуживаемых им и при положительном результате, отправляет на него уведомление о зачислении средств;
7. Через какое-то время (обычно моментально) на указанной номер приходит уведомление о пополнении баланса мобильного телефона. Профит!

Однако, если при вводе номера была допущена ошибка, данное уведомление получит лицо, отличное от нашего пользователя…


---

### Задание 3. SQL vs NoSQL

##Ответ:

Преимущества SQL-систем по отношению к NoSQL:

1. Язык запросов SQL, разрабатываемый с 1980-х и имеющий стандарты;
2. Наличие транзакций (и ACID);
3. Обеспечение целостности данных;
4. Кроссплатформенная реализация;
5. Четкая структура таблиц данных;
6. Всегда ожидаемый результат выполнения запросов.


---

### Задание 4. Кластеры

##Ответ:

Для большого количества вычислений при работе с огромным количеством данных, я бы выбрал NoSQL, использовав все ее преимущества, такие как:

1. Гибкость;
2. Масштабируемость;
3. Высокая производительность;
4. Широкие функциональные возможности.

Исходя из большого количества машин и того, что они все связаны друг с другом, нам важны:

1. Устойчивость к распаду на секции;
2. Доступность.

Соответственно, согласно PACELС, считаю уместным использовать модель PA, следовательно, решение – MongoDB.


---
