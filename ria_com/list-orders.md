#### Перелік замовлень 

Щоб отримати список замовлень, потрібно надіслати GET запит на адресу [https://developers.ria.com/ria/basket/orders/?user_id=*&api_key=YOUR_API_KEY](https://developers.ria.com/ria/basket/orders/?user_id=*&api_key=YOUR_API_KEY). Де **user_id** - потрібно вказати Ваш id.

````javascript
  curl -X GET https://developers.ria.com/ria/basket/orders?user_id=*api_key=YOUR_API_KEY
 ````
 Результат буде орієнтовно наступним:

```javascript
{
   "status":true,
   "total":2,
   "orders":[
     {
       "order_id":212121,                      // id замовлення
       "status":6,                            // Статус "Видалені"
       "total_order_sum":100,                 // Загальна сума замовлення
       "created_at":"2023-01-11 03:39:30",    // Час створення
       "recipient":{
         "user_id":000000,                    // id користувача
         "name":"Андрій Сергійович",
         "email":"mail@gmail.com",
         "phone":"......"                     // Телефон
       },
       "delivery":{                           // Доставка
          "state_id":1,                       // id Області
         "city_id":1,                         // id Міста
         "address":"Вінницька область, Вінниця",
         "service":"DHL"                      // Служба доставки
         "department":"Відділення №1: вулиця Соборна, 15; оф. 6"  // Інформація про відділення
       },
       "items":[
         {
           "adv_id":122724239,                 // id оголошення
           "name":"Диффузор 1j0121207m",
           "price":100,                       // Ціна
           "count":1,                         // Кількість
           "note":""                          // Нотатки
           "vendor_code":"",                  // Код постачальника
           "catalog_numbers":""               // Каталожний номер
         }
       ]
     },
     ...
   ]
```



