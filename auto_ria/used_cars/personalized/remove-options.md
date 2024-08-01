### Видалення опцій

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

Для видалення опцій оголошення, Вам необхідно відправити **DELETE** запит такого формату:
````javascript
curl -X DELETE "https://developers.ria.com/auto/used/autos/advertisementId/options/ids?user_id=Ваш ID&api_key=YOUR_API_KEY" -H "accept: application/json"
`````
де *user_id* - Ваш ID в системі RIA.com, *advertisementId* - ID потрібного Вам оголошення, "id": - ID потрібної Вам опції, *api_key* - Ваш ключ.

**Приклад запиту**
````javascript
curl -X DELETE "https://developers.ria.com/auto/used/autos/20438832/options/125,525,481?user_id=7069830&api_key=YOUR_API_KEY" -H "accept: application/json"`
````
