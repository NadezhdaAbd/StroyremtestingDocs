* Тестовые данные: Позитивная проверка. Блок “Редактировать данные” - совпадение с макетом.

	тестовый сервер - https://test2.stroyrem-nn.ru/   продовый сервер - https://stroyrem-nn.ru/

* Предусловие: пользователь авторизован, открыт «Личный кабинет»

* Шаги:
1.	Сверить блок "Редактировать данные" с макетом

* Ожидаемый результат: в блоке есть:
	- аватар с начальной буквой имени (если фото не загружено) или фото
	- "+" на аватаре (если фото не загружено) / ? (если фото загружено)
	- имя
	- ссылка "Редактировать данные" (на таче ещё есть стрелка >)
	- прогресс заполнения профиля данными:
		- линия прогресса из 5 точек, меняют цвет по мере заполнения профиля
		- указано число процентов "Заполнено" (например 90% заполнено) 

* Постусловие: удалить тестовые данные

Автор: Надежда

* Отчет о тестировании
  
Тестовый сервер
| Дата | Время | Версия браузера Десктоп | Результат/Баг в Трелло Десктоп|  Версия браузера и ОС Тач |Результат/Баг в Трелло Тач| Дата релиза| QA  |
| --- | --- | --- | --- |  --- | --- | --- | --- |   
| 08.09.23 | 19:00 | Chrome версия 116.0.5845.180 Firefox версия 117.0 | FAIL https://trello.com/c/rzHN8yeC/505  | Chrome версия 116.0.5845.163 MIUI 12.5.13 | FAIL https://trello.com/c/rzHN8yeC/505 | 03.09.23 | Надежда |  

Продовый сервер
| Дата | Время | Версия браузера Десктоп | Результат/Баг в Трелло Десктоп|  Версия браузера и ОС Тач |Результат/Баг в Трелло Тач| Дата релиза| QA |
| --- | --- | --- | --- |  --- | --- | --- | --- |   
| 08.09.23 | 19:02 | Chrome версия 116.0.5845.180 Firefox версия 117.0 | FAIL https://trello.com/c/rzHN8yeC/505 | Chrome версия 116.0.5845.163 MIUI 12.5.13 | FAIL https://trello.com/c/rzHN8yeC/505 | 03.09.23 | Надежда |