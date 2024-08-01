### Список оголошень користувача

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

Щоб отримати список оголошень, Вам необхідно виконати GET запит такого формату:

https://developers.ria.com/auto/used/autos/ids?user_id=Ваш ID в системі RIA.com&api_key=YOUR_API_KEY

або 
````javascript
curl -X GET "https://developers.ria.com/auto/used/autos/ids?user_id=Ваш ID&api_key=YOUR_API_KEY" -H "accept: application/json"
`````
де *user_id* - Ваш ID в системі RIA.com, *api_key* - Ваш ключ.

**Приклад запиту**
````javascript
curl -X GET "https://developers.ria.com/auto/used/autos/ids?user_id=7069830&api_key=YOUR_API_KEY" -H "accept: application/json"
`````
**Приклад успішної відповіді:**

```json
{
  "active": {
    "moderated": [

    ],
    "notModerated": [

    ]
  },
  "draft": [

  ],
  "awaitingPayment": [

  ],
  "archive": [
    20438832,
    20445742
  ]
}
```
Розшифрування параметрів:
 - *active* - Активні оголошення
 - *moderated* - Оголошення перебувають на модерації
 - *notModerated* - Оголошення не відмодеровано
 - *draft* - Оголошення знаходяться в чернетках
 - *awaitingPayment* - Оголошення очікують оплати
 - *archive* - Оголошення в архіві

