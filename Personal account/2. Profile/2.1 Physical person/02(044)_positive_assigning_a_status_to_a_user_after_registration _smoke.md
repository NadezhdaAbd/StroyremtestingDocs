* Тестовые данные: Позитивная проверка. Присвоение статуса пользователю после регистрации.

	тестовый сервер - https://test2.stroyrem-nn.ru/   продовый сервер - https://stroyrem-nn.ru/

* Предусловие: открыта Главная страница, новый пользователь без регистрации

* Шаги:
1.	Нажать в хедере на "Профиль"
2.	В выпадающем окне нажать "Регистрация"
3.	Заполнить форму регистрации физического лица валидными данными
4.	Нажать "Зарегистрироваться"

* Ожидаемый результат:
	1. открывается "Личный кабинет", в блоке "Ваш статус" выставлен статус "Стартовый"
	2. в блоке с информацией о покупках и баллах выставлен тип цен "ОПТ2"
	
* Постусловие: удалить тестовые данные

Автор: Надежда

* Отчет о тестировании
  
Тестовый сервер
| Дата | Время | Версия браузера Десктоп | Результат/Баг в Трелло Десктоп|  Версия браузера и ОС Тач |Результат/Баг в Трелло Тач| Дата релиза| QA  |
| --- | --- | --- | --- |  --- | --- | --- | --- |   
| 18.07.23 | 20:18 | Chrome версия 114.0.5735.199 Firefox версия 115.0.2 | PASS | Chrome версия 114.0.5735.196 MIUI 12.5.13 | PASS | 16.06.23 | Надежда |  

Продовый сервер
| Дата | Время | Версия браузера Десктоп | Результат/Баг в Трелло Десктоп|  Версия браузера и ОС Тач |Результат/Баг в Трелло Тач| Дата релиза| QA |
| --- | --- | --- | --- |  --- | --- | --- | --- |   
| 18.07.23 | 20:23 | Chrome версия 114.0.5735.199 Firefox версия 115.0.2 | PASS | Chrome версия 115.0.5790.171 MIUI 12.5.13 | PASS | 16.06.23 | Надежда |
| 14.08.23 | 13:30 | Yandex версия 23.7.2.768  Microsoft Edge версия 115.0.1901.204 | PASS | Chrome версия 114.0.5735.196 Samsung Galaxy A50 | PASS | 13.08.23 | Наталья К. |   