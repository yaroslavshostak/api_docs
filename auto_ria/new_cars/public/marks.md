## Марки

Марки залежать від типів транспорту. Тому для того, щоб отримати список марок, необхідно надіслати GET запит за адресою `https://developers.ria.com/auto/new/marks?category_id=id&api_key=YOUR_API_KEY`, де *category_id* - ідентифікатор типу транспорту, *api_key*- Ваш ключ.

Наприклад, для легкових автомобілів ([https://developers.ria.com/auto/new/marks?category_id=1&api_key=YOUR_API_KEY](https://developers.ria.com/auto/new/marks?category_id=1&api_key=YOUR_API_KEY)), результат буде наступним:
```javascript
[ 
 {
  "category_id":1,
  "cnt":1,
  "country_id":0,
  "eng":"abarth",
  "marka_id":5166,
  "name":"Abarth",
  "slang":"Абарт",
  "value":5166
 },
 {
  "category_id":1,
  "cnt":369,
  "country_id":392,
  "eng":"acura",
  "marka_id":98,
  "name":"Acura",
  "slang":"Акура",
  "value":98
 },
]  
.......
```
