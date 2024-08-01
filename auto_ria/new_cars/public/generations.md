## Покоління моделі нового авто

  **Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**
  
Покоління залежить від моделі нового авто. Отже список поколінь можна отримати надіславши GET запит на адресу `https://developers.ria.com/auto/new/generations?model_id=id&api_key=YOUR_API_KEY`, де  *model_id* - модель обраного авто, *api_key*- Ваш ключ.

Наприклад, для моделі BMW X6 ([https://developers.ria.com/auto/new/generations?model_id=2153&api_key=YOUR_API_KEY](https://developers.ria.com/auto/new/generation?model_id=2153&api_key=YOUR_API_KEY)), список поколінь буде таким:

```javascript
[
 {
  "eng":"e71-fl",
  "generation_id":432,
  "marka_id":9,
  "model_id":2153,
  "name":"E71 (FL)",
  "year_from":2012,
  "year_to":2014
 },
 {
  "eng":"f16",
  "generation_id":433,
  "marka_id":9,
  "model_id":2153,
  "name":"F16",
  "year_from":2014,
  "year_to":0
 },
 {
  "eng":"e71",
  "generation_id":3275,
  "marka_id":9,
  "model_id":2153,
  "name":"E71",
  "year_from":2008,
  "year_to":2011
 },
 {
  "eng":"g06",
  "generation_id":7541,
  "marka_id":9,
  "model_id":2153,
  "name":"G06",
  "year_from":2019,
  "year_to":0
 }
]
````
