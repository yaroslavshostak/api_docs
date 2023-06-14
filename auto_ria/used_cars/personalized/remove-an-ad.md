### Видалення оголошення

Для видалення оголошення, Вам необхідно відправити **DELETE** запит такого формату:
````javascript
curl -X DELETE "https://developers.ria.com/auto/used/autos/advertisementId?user_id=Ваш ID&reason_id=id причини видалення&api_key=YOUR_API_KEY" -H "accept: application/json"
`````
де *user_id* - Ваш ID в системі RIA.com, *advertisementId* - ID потрібного Вам оголошення, *reason_id* - причина видалення, *api_key* - Ваш ключ.

**reason_id** складається з 4 категорій:
- **reason_id**=**4** - Авто продано за допомогою AUTO.RIA.com
- **reason_id**=**5** - Авто продано в іншому місці
- **reason_id**=**6** - Я хочу розмістити оголошення знову
- **reason_id**=**7** - Я передумав продавати автомобіль

**Приклад запиту**
````javascript
curl -X DELETE "https://developers.ria.com/auto/used/autos/20460133?user_id=7069830&reason_id=7&api_key=YOUR_API_KEY" -H "accept: application/json"`
`````

