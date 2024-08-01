### Статистика оголошення

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

Щоб отримати статистику про оголошення, Вам необхідно виконати GET запит такого типу:

https://developers.ria.com/auto/used/autos/advertisementId/statistic?user_id=Ваш ID&api_key=YOUR_API_KEY

або 
````javascript
curl -X GET "https://developers.ria.com/auto/used/autos/advertisementId/statistic?user_id=Ваш ID&api_key=YOUR_API_KEY" -H "accept: application/json"
`````
де *user_id* - Ваш ID в системі RIA.com, *advertisementId* - ID потрібного Вам оголошення, *api_key* - Ваш ключ.

**Приклад запиту**
````javascript
curl -X GET "https://developers.ria.com/auto/used/autos/20268839/statistic?user_id=7069830&api_key=YOUR_API_KEY" -H "accept: application/json""`
````
**Приклад успішної відповіді:**

```json
{
  "views": 329,
  "clicks": 24
}
```
Розшифрування параметрів:

- *views* - Кількість переглядів оголошення
- *clicks* - Кількість відкриттів номера телефону

 
