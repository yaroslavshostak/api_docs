### Додавання опцій

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

Для додавання опцій в оголошення, Вам необхідно виконати PUT запит такого виду:
````javascript
curl -X POST "https://developers.ria.com/auto/used/autos/advertisementId/options?user_id=Ваш ID&api_key=YOUR_API_KEY" -H "accept: application/json" -H "content-type: application/json" -d "[ { \"id\": ID опції }]"
````
де *user_id* - Ваш ID в системі RIA.com, *advertisementId* - ID потрібного Вам оголошення, "id": - ID потрібної Вам опції, *api_key* - Ваш ключ.

**Приклад запиту**
````javascript
curl -X POST "https://developers.ria.com/auto/used/autos/20438832/options?user_id=7069830&api_key=YOUR_API_KEY" -H "accept: application/json" -H "content-type: application/json" -d "[ { \"id\": 525 }]"`
`````
**Приклад успішної відповіді:**
````json
{"message":"Ok",

"errors":[],

"success":true}
````

