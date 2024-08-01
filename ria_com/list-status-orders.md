#### Перелік статусів замовлень

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

Щоб отримати список типів статусів, потрібно надіслати GET запит на адресу [https://developers.ria.com/ria/basket/status?api_key=YOUR_API_KEY](https://developers.ria.com/ria/basket/status?api_key=YOUR_API_KEY). Результат буде приблизно таким:
````javascript
 curl -X GET https://developers.ria.com/ria/basket/status?api_key=YOUR_API_KEY
````
```javascript
{
  "status": true,
  "data": [
    {
      "id": 0,
      "name": "Нові та Невиконані"
    },
    {
      "id": 1,
      "name": "Bиконані"
    },
    {
      "id": 2,
      "name": "Hевиконані"
    },
    {
      "id": 6,
      "name": "Видалені"
    },
    {
      "id": 4,
      "name": "Всі"
    },
    {
       "id": 7,
       "name": "Зворотній дзвінок"
     }
  ]
}
```
