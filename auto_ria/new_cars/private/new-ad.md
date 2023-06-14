## Створення нового оголошення 

Для створення нового оголошення, вам необхідно виконати **POST** запит такого виду:
 
`curl -X POST "https://developers.ria.com/auto/new/autos?user_id=4784009&marka_id=id&model_id=id&`
`base_id=id&equip_id=id&currency_id=id&price=цена&in_stock=id&test_drive=id&api_key=YOUR_API_KEY"`
` -H "accept: application/json"`


Обов'язковими параметрами є:
- *user_id* -  Ваш ID у системі RIA.com
- *marka_id* - Марка автомобіля
- *model_id* -  Модель автомобіля
- *base_id* - Модифікація (бази) за типом кузова
- *equip_id* - Комплектація автомобіля
- *currency_id* - Валюта в якій продаєте автомобіль (1 - долари США, 2 - євро, 3 - гривня)

Додаткові параметри:
- *price* - Ціна
- *auto_note* - Опис
- *version* - Версія (приклад 2.0 TDI)
- *in_stock* - У наявності (1 - в наявності, 0 - немає в наявності)
- *test_drive* - Можливість пройти тест драйв (1 - є можливість, 0 - немає можливості)

**Приклад запиту**

`curl -X POST "https://developers.ria.com/auto/new/autos?user_id=4784009&marka_id=9&model_id=2153&`
`base_id=9036&equip_id=79274&currency_id=1&price=50000&in_stock=1&test_drive=1&api_key=YOUR_API_KEY"`
` -H "accept: application/json"`

**Приклад успішної відповіді:**

```javascript
{
  "num_rows": 1,
  "last_insert_id": 1696388
}
```
