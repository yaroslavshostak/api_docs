## Видалення оголошення

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

Для видалення оголошення, Вам необхідно відправити **DELETE** запит такого вигляду:

`curl -X DELETE "https://developers.ria.com/auto/new/autos?user_id=id&auto_id=id&api_key=YOUR_API_KEY"`
` -H "accept: application/json"`

, де *auto_id* - ваш ID у системі RIA.com, *auto_id* - id потрібного Вам оголошення, *api_key* - ваш ключ.

**Приклад запиту**

`curl -X DELETE "https://developers.ria.com/auto/new/autos?user_id=4784009&auto_id=1696388&`
`api_key=YOUR_API_KEY" -H "accept: application/json"`

**Приклад успішної відповіді:**

```javascript
{"num_rows":1,
"last_insert_id":0}
```
