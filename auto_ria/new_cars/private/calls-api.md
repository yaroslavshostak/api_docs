## Отримання даних про дзвінок

### GET API для отримання даних про дзвінок

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

Щоб отримати дані про дзвінки, вам необхідно виконати GET-запит такого формату:

https://developers.ria.com/auto/new/calls_stat?user_id=Ваш_ID&from=ДАТА_ПОЧАТКУ_ВИБІРКИ&to=ДАТА_КІНЦЯ_ВИБІРКИ&api_key=YOUR_API_KEY

або
````javascript
curl -X GET "https://developers.ria.com/auto/new/calls_stat?user_id=Ваш_ID&from=ДАТА_ПОЧАТКУ_ВИБІРКИ&to=ДАТА_КІНЦЯ_ВИБІРКИ&api_key=YOUR_API_KEY" -H "accept: application/json"
````
 де *user_id* - Ваш ID в системі RIA.com; *from*, *to* - фільтр за діапазоном дат (рік - місяць - день); *api_key* - Ваш ключ.

**Приклад запиту**
````javascript
curl -X GET "https://developers.ria.com/auto/new/calls_stat?from=2021-06-01&to=2021-07-31&user_id=1505029&api_key=YOUR_API_KEY" -H "accept: application/json"
````
**Приклад успішної відповіді:**
[1]: 
```json
[
  {
    "call_id": 22346351,
    "caller_phone": "0951174074",
    "date": "2021-07-31T15:57:01",
    "destination_phone": "0731375686",
    "duration": 0,
    "link": "",
    "marka": "Acura",
    "marka_id": 98,
    "model": "MDX",
    "model_id": 955,
    "phone": "0730946407",
    "price": 0,
    "status": "CANCEL",
    "waighting": 11
  },
  {
    "call_id": 22345654,
    "caller_phone": "0968404829",
    "date": "2021-07-31T14:42:24",
    "destination_phone": "0731375686",
    "duration": 0,
    "link": "",
    "marka": null,
    "marka_id": 0,
    "model": null,
    "model_id": 0,
    "phone": "0504103684",
    "price": 0,
    "status": "BUSY",
    "waighting": 48
  },
  {
    "call_id": 22326708,
    "caller_phone": "0674294559",
    "date": "2021-07-30T17:00:12",
    "destination_phone": "0731375686",
    "duration": 57,
    "link": "https://track.ria.com/call_link/56w456gw45v5765ee5ser_w45/2021/07/30/380731375686=380674294559=17-00-12.wav",
    "marka": "Acura",
    "marka_id": 98,
    "model": "MDX",
    "model_id": 955,
    "phone": "0935063003",
    "price": 0,
    "status": "ANSWER",
    "waighting": 22
  },
  {
    "call_id": 22325473,
    "caller_phone": "0931426064",
    "date": "2021-07-30T15:30:21",
    "destination_phone": "0731375686",
    "duration": 0,
    "link": "",
    "marka": "Acura",
    "marka_id": 98,
    "model": "MDX",
    "model_id": 955,
    "phone": "0936073263",
    "price": 0,
    "status": "CANCEL",
    "waighting": 44
  }
]   
````
Розшифрування параметрів:

- *call_id* - Унільний ID дзвінка
- *caller_phone* - Номер телефону, з якого був дзвінок
- *date* - Дата і час дзвінка
- *destination_phone* - Реальний номер на який переадресовувався дзвінок
- *duration* - Тривалість дзвінка в секундах
- *link* - Посилання на запис розмови
- *marka* - Марка, якою цікавилися під час розмови
- *marka_id* - ID марки
- *model* - Модель, якою цікавилися під час розмови
- *model_id* - ID моделі
- *phone* - Підмінний номер телефону, на який дзвонили
- *status* - Статус дзвінка (ANSWER, NOANSWER, CANCEL, BYSY, FAILED, CONGESTION)
- *waighting* - Час у секундах, перш ніж відбулося з'єднання

______

### POST API для отримання даних про дзвінок

Другий спосіб передачі даних про дзвінок:

1. У вас є back-end із веб-сервером.
2. Ви передаєте свій url API (наприклад: https://your_site.com/api/call/call_from_auto_ria).
3. Щойно клієнт ставить слухавку, на цю адресу ми відправляємо всі дані (список параметрів в [п.1][1]).
4. Ви обробляєте отримані дані на своєму боці.

