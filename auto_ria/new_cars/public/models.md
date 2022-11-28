## Моделі

Моделі залежать від типів транспорту і марок. Відповідно список марок можна отримати за адресою `https://developers.ria.com/auto/new/models?marka_id=id&category_id=id&api_key=YOUR_API_KEY`, де *category_id* - ідентифікатор типу транспорту, а *marka_id* - ідентифікатор марки, *api_key*- Ваш ключ.

Наприклад, для легкового автомобіля BMW ([https://developers.ria.com/auto/new/models?marka_id=9&category_id=1&api_key=YOUR_API_KEY](https://developers.ria.com/auto/new/models?marka_id=9&category_id=1&api_key=YOUR_API_KEY)), список моделей буде наступним:
```javascript
[
  {
   "category_id":"1",
   "count":0,
   "eng":"ix1",
   "marka_id":9,
   "model_id":63528,
   "name":"iX1",
   "parent_id":0,
   "slang":null,
   "value":63528
  },
  {
  "category_id":"1",
  "count":0,
  "eng":"1500",
  "marka_id":9,
  "model_id":63521,
  "name":"1500",
  "parent_id":0,
  "slang":null,
  "value":63521
  },
]  
.......
````
