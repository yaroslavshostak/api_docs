## Редагування оголошення

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

Для редагування основної інформації оголошення, вам необхідно надіслати **PUT** запит такого типу:

`curl -X PUT "https://developers.ria.com/auto/new/autos?user_id=Ваш id&auto_id=id&`
`currency_id=id&price=Ціна&auto_note=Test&in_stock=id&test_drive=id&api_key=YOUR_API_KEY"`
` -H "accept: application/json" -H "Content-Length: 0"`

Обов'язковими параметрами є:
- *user_id* - Ваш ID у системі RIA.com
- *auto_id* - ID потрібного Вам оголошення
- *currency_id* - Валюта в якій продаєте автомобіль (1 - долари США, 2 - євро, 3 - гривня)
- *Content-Length* - розмір документа, що повертається (Content-Length: 0)

Додаткові параметри:
- *price* - Ціна
- *auto_note* - Опис
- *version* - Версія ( наприклад 2.0 TDI)
- *in_stock* - У наявності   (1 - у наявності, 0 - немає в наявності)
- *test_drive* - Можливість пройти тест драйв (1 - є можливість, 0 - немає можливості)
- 
**Приклад запиту**

`curl -X PUT "https://developers.ria.com/auto/new/autos?user_id=4784009&auto_id=1696388&currency_id=2&`
`price=55000&auto_note=Test&in_stock=0&test_drive=0&api_key=YOUR_API_KEY"`
` -H "accept: application/json" -H "Content-Length: 0"`

**Приклад успішної відпвовіді:**

```javascript
{"num_rows":1,
"last_insert_id":0}
```
