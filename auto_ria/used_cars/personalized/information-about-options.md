### Отримання інформації про опції оголошення

Щоб отримати інформацію про опції оголошення, Вам необхідно виконати GET запит такого формату:

https://developers.ria.com/auto/used/autos/advertisementId/options?user_id=Ваш ID&api_key=YOUR_API_KEY

або `curl -X GET "https://developers.ria.com/auto/used/autos/advertisementId/options?user_id=Ваш ID&api_key=YOUR_API_KEY" -H "accept: application/json"`

де *user_id* - Ваш ID в системі RIA.com, *advertisementId* - ID потрібного Вам оголошення, *api_key* - Ваш ключ.

**Приклад запиту**
````javascript
curl -X GET "https://developers.ria.com/auto/used/autos/20438832/options?user_id=7069830&api_key=YOUR_API_KEY" -H "accept: application/json"
````
**Приклад успішної відповіді:**
```json
[
  {
    "id": 125
  },
  {
    "id": 137
  },
  {
    "id": 188
  },
  {
    "id": 189
  },
  {
    "id": 190
  },
  {
    "id": 191
  },
  {
    "id": 211
  },
  {
    "id": 217
  },
  {
    "id": 225
  },
  {
    "id": 303
  },
  {
    "id": 354
  },
  {
    "id": 355
  },
  {
    "id": 437
  },
  {
    "id": 463
  },
  {
    "id": 481
  },
  {
    "id": 525
  }
]
```

Для розшифровки отриманих параметрів можна використовувати сервіс [Опції](https://api-docs-v2.readthedocs.io/ru/latest/auto_ria/used_cars/options/options.html?highlight=%D0%BE%D0%BF%D1%86%D1%96%D1%97#section-1)

