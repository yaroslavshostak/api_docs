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

Для розшифровки отриманих параметрів можна використовувати сервіс [Опції](https://github.com/ria-com/auto-ria-rest-api/blob/master/AUTO_RIA_API/README.md#user-content-%D0%9E%D0%BF%D1%86%D0%B8%D0%B8)

 Повний опис сервісу "Отримання інформації про опції оголошення" описаний за допомогою стандарту **DeFacto swagger 2.0** [тут](http://swagger.ria.com/ui/?api=auto/advertisements#/)
