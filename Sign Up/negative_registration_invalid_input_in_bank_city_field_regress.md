Regjur 27

Регистрация нового пользователя (юр лицо) с введенными невалидными данными в поле "Город банка" (данные о счете организации)

* Тестовые данные: 
  
  Предусловия:
  
  1. Создан тестовый электронный ящик(и)
  
  2. Открыта форма регистрации и выбрана вкладка "Юридическое лицо" 
     
     (ссылка на прод [Регистрация](https://stroyrem-nn.ru/user/register) и на тест [Регистрация](https://test2.stroyrem-nn.ru/user/register))
  
  3. Все поля заполнены валидными данными, кроме поля "Город банка" (данные о счете организации)

* Шаги:
1. Оставить не обязательное поле для заполнения "Город банка" (данные о счете организации) пустым и нажать кнопку "Зарегистрироваться"
   
   **ОР:** Происходит успешная регистрация нового пользователя (юр лицо), открывается профиль пользователя

2. Ввести в поле "Город банка" (данные о счете организации) специальные символы !@#$%^&*()_+<> и нажать кнопку "Зарегистрироваться"
   
   **ОР:** Поле "Город банка" в рамке красного цвета и появляется надпись "Название не может содержать специальные символы !@#$%^&*()_+<>?/:;"

3. Ввести в поле "Город банка" (данные о счете организации) вредоносный код <script>alert(“I hacked this!”)</script> и нажать кнопку "Зарегистрироваться"
   
   **ОР:** Поле "Город банка" в рамке красного цвета и появляется надпись "Название не может содержать специальные символы !@#$%^&*()_+<>?/:;"

4. Ввести в поле "Город банка" (данные о счете организации) sql инъекцию FOO'); DROP TABLE NUMBER и нажать кнопку "Зарегистрироваться"
   
   **ОР:** Поле "Город банка" в рамке красного цвета и появляется надпись "Название не может содержать специальные символы !@#$%^&*()_+<>?/:;"

5. Ввести в поле "Город банка" (данные о счете организации) пробелы и нажать кнопку "Зарегистрироваться"
   
   **ОР:** Поле "Город банка" в рамке красного цвета и появляется надпись "Поле не может содержать одни пробелы"
* Постусловия: удалить тестовые данные на тестовом сервере/выйти из профиля, если регистрация проходит успешно

Автор: Татьяна

* Тестовый сервер 

Тест выполнен

|  №  | Дата       | Время |           Версия браузера           |        Результат/Баг в            |             Версия браузера и       |           Результат/Баг в          |  Дата  |  Имя   |
								          Десктоп		                   Трелло Десктоп		                        ОС Тач			                  Трелло Тач	          Релиза
| --- | ---------- | ----- |-------------------------------------| ---------------------------------- | ---------------------------------- | ---------------------------------- | ------| ------  |
| 1   | 2023-08-02 | 13:20 |Chrome 115.0.5790.110 Firefox 115.0.3| PASS      						  | Huawei Mate 10 PRO EMUI 12.0.0.225 | PASS      						    | 04.07 | Татьяна |
| 2   | 2023-08-02 | 13:33 |Chrome 115.0.5790.110 Firefox 115.0.3| FAIL https://trello.com/c/9d312LaU | Huawei Mate 10 PRO EMUI 12.0.0.225 | FAIL https://trello.com/c/9d312LaU | 04.07 | Татьяна |
| 3   | 2023-08-02 | 13:43 |Chrome 115.0.5790.110 Firefox 115.0.3| FAIL https://trello.com/c/NXVgBXpM | Huawei Mate 10 PRO EMUI 12.0.0.225 | FAIL https://trello.com/c/NXVgBXpM | 04.07 | Татьяна |
| 4   | 2023-08-02 | 13:50 |Chrome 115.0.5790.110 Firefox 115.0.3| FAIL https://trello.com/c/KVEOrLyL | Huawei Mate 10 PRO EMUI 12.0.0.225 | FAIL https://trello.com/c/KVEOrLyL | 04.07 | Татьяна |
| 5   | 2023-08-02 | 14:00 |Chrome 115.0.5790.110 Firefox 115.0.3| FAIL https://trello.com/c/GUPIBGTf | Huawei Mate 10 PRO EMUI 12.0.0.225 | FAIL https://trello.com/c/GUPIBGTf | 04.07 | Татьяна |
| --- | ---------- | ----- |-------------------------------------| ---------------------------------- | ---------------------------------- | ---------------------------------- | ------| ------  |
| 1   | 2023-08-15 | 20:20 |Chrome 116.0.5845.97 Yandex 23.7.2.765| PASS      						  | Xiaomi Mi 9 Lite MIUI 12.5.2       | PASS      						    | 13.08 | Сабина  |
| 2   | 2023-08-16 | 10:00 |Chrome 116.0.5845.97 Yandex 23.7.2.765| FAIL https://trello.com/c/9d312LaU| Xiaomi Mi 9 Lite MIUI 12.5.2       | FAIL https://trello.com/c/9d312LaU | 13.08 | Сабина  |
| 3   | 2023-08-16 | 10:20 |Chrome 116.0.5845.97 Yandex 23.7.2.765| FAIL https://trello.com/c/NXVgBXpM | Xiaomi Mi 9 Lite MIUI 12.5.2      | FAIL https://trello.com/c/NXVgBXpM | 13.08 | Сабина |
| 4   | 2023-08-16 | 10:25 |Chrome 116.0.5845.97 Yandex 23.7.2.765| FAIL https://trello.com/c/KVEOrLyL | Xiaomi Mi 9 Lite MIUI 12.5.2      | FAIL https://trello.com/c/KVEOrLyL | 13.08 | Сабина |
| 5   | 2023-08-16 | 10:30 |Chrome 116.0.5845.97 Yandex 23.7.2.765| FAIL https://trello.com/c/GUPIBGTf | Xiaomi Mi 9 Lite MIUI 12.5.2      | FAIL https://trello.com/c/GUPIBGTf | 13.08 | Сабина |

* Продовый сервер

Тест выполнен

|  №  | Дата       | Время |           Версия браузера           |        Результат/Баг в            |             Версия браузера и       |           Результат/Баг в          |  Дата  |  Имя   |
								          Десктоп		                   Трелло Десктоп		                        ОС Тач			                  Трелло Тач	          Релиза
| --- | ---------- | ----- |-------------------------------------| ---------------------------------- | ---------------------------------- | ---------------------------------- | ------| ------  |
| 1   | 2023-08-02 | 13:20 |Chrome 115.0.5790.110 Firefox 115.0.3| PASS      						  | Huawei Mate 10 PRO EMUI 12.0.0.225 | PASS      						    | 04.07 | Татьяна |
| 2   | 2023-08-02 | 13:33 |Chrome 115.0.5790.110 Firefox 115.0.3| FAIL https://trello.com/c/9d312LaU | Huawei Mate 10 PRO EMUI 12.0.0.225 | FAIL https://trello.com/c/9d312LaU | 04.07 | Татьяна |
| 3   | 2023-08-02 | 13:43 |Chrome 115.0.5790.110 Firefox 115.0.3| FAIL https://trello.com/c/NXVgBXpM | Huawei Mate 10 PRO EMUI 12.0.0.225 | FAIL https://trello.com/c/NXVgBXpM | 04.07 | Татьяна |
| 4   | 2023-08-02 | 13:50 |Chrome 115.0.5790.110 Firefox 115.0.3| FAIL https://trello.com/c/KVEOrLyL | Huawei Mate 10 PRO EMUI 12.0.0.225 | FAIL https://trello.com/c/KVEOrLyL | 04.07 | Татьяна |
| 5   | 2023-08-02 | 14:00 |Chrome 115.0.5790.110 Firefox 115.0.3| FAIL https://trello.com/c/GUPIBGTf | Huawei Mate 10 PRO EMUI 12.0.0.225 | FAIL https://trello.com/c/GUPIBGTf | 04.07 | Татьяна |
| --- | ---------- | ----- |-------------------------------------| ---------------------------------- | ---------------------------------- | ---------------------------------- | ------| ------  |
| 1   | 2023-08-15 | 20:25 |Chrome 116.0.5845.97 Yandex 23.7.2.765| PASS      						  | Xiaomi Mi 9 Lite MIUI 12.5.2       | PASS      						    | 13.08 | Сабина  |
| 2   | 2023-08-16 | 10:40 |Chrome 116.0.5845.97 Yandex 23.7.2.765| FAIL https://trello.com/c/9d312LaU| Xiaomi Mi 9 Lite MIUI 12.5.2       | FAIL https://trello.com/c/9d312LaU | 13.08 | Сабина  |
| 3   | 2023-08-16 | 10:45 |Chrome 116.0.5845.97 Yandex 23.7.2.765| FAIL https://trello.com/c/NXVgBXpM | Xiaomi Mi 9 Lite MIUI 12.5.2      | FAIL https://trello.com/c/NXVgBXpM | 13.08 | Сабина |
| 4   | 2023-08-16 | 10:50 |Chrome 116.0.5845.97 Yandex 23.7.2.765| FAIL https://trello.com/c/KVEOrLyL | Xiaomi Mi 9 Lite MIUI 12.5.2      | FAIL https://trello.com/c/KVEOrLyL | 13.08 | Сабина |
| 5   | 2023-08-16 | 10:55 |Chrome 116.0.5845.97 Yandex 23.7.2.765| FAIL https://trello.com/c/GUPIBGTf | Xiaomi Mi 9 Lite MIUI 12.5.2      | FAIL https://trello.com/c/GUPIBGTf | 13.08 | Сабина |