## Комплектації авто за модифікацією

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**
    
Комплектації авто залежать від модифікації (бази). Отримати їх список можна надіславши GET запит за адресою `https://developers.ria.com/auto/new/equips?base_id=id&api_key=YOUR_API_KEY`, де *base_id* - id модифікації (бази), *api_key*- Ваш ключ.

Наприклад, для моделі BMW X6 E71 50i AT (407 к.с.) xDrive  (https://developers.ria.com/auto/new/equips?base_id=9036&api_key=YOUR_API_KEY) список комплектації буде таким:

```javascript
[
 {
  "base_id":9036,
  "cnt":0,
  "equip_id":79274,
  "min_price":null,
  "name": "Base",
  "year":"2022"
 }
]

```
