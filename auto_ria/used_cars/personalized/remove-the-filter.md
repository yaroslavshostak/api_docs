### Видалення існуючого фільтра на обмін

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

Для видалення існуючого фільтра на обмін, Вам необхідно виконати DELETE запит такого виду:
````javascript
curl -X DELETE "https://developers.ria.com/auto/used/autos/advertisementId/exchangeFilter/filterId?user_id=Ваш ID&api_key=c" -H "accept: application/json"`
`````
, де *user_id* - Ваш ID у системі RIA.com, *advertisementId* - ID потрібного Вам оголошення, *filterId* - ID обраного Вами фільтра, *api_key* - Ваш ключ.

**Приклад запиту**
````javascript
curl -X DELETE "https://developers.ria.com/auto/used/autos/20438832/exchangeFilter/2930510?user_id=7069830&api_key=YOUR_API_KEY" -H "accept: application/json"`
`````
