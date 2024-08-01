### Отримання фільтрів на обмін за вашим оголошенням

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

Для отримання опцій в оголошенні, Вам необхідно виконати GET запит такого типу:

https://developers.ria.com/auto/used/autos/advertisementId/exchangeFilters?user_id=ВашID&api_key=YOUR_API_KEY

або 
````javascript
curl -X GET "https://developers.ria.com/auto/used/autos/advertisementId/exchangeFilters?user_id=Ваш ID&api_key=YOUR_API_KEY" -H "accept: application/json"
`````
, де *user_id* - Ваш ID в системі RIA.com, *advertisementId* - ID потрібного Вам оголошення, *api_key* - Ваш ключ.

**Приклад запиту**
````javascript
curl -X GET "https://developers.ria.com/auto/used/autos/20438832/exchangeFilters?user_id=7069830&api_key=YOUR_API_KEY" -H "accept: application/json"
`````
**Приклад успішної відповіді:**

````json

[
  {
    "id": 2930510,   // Id доданого фільтра
    "brand": {
      "id": 6
    },
    "model": {
      "id": 3460
    },
    "year": {
      "lte": 2013,
      "gte": 2010
    },
    "category": {
      "id": 1
    },
    "body": {
      "id": 3
    }
  }
]
````


