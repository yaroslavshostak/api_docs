## Типи кузова в поколінні нових авто

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**
    
Тип авто кузова залежить від покоління авто. Тому для того, щоб отримати список типів кузова, необхідно надіслати GET запит на адресу `https://developers.ria.com/auto/new/generation_bodystyles?generation_id=id&api_key=YOUR_API_KEY` , де *generation_id* - покоління авто, *api_key*- Ваш ключ.

Наприклад, для моделі BMW X6 у поколінні E71 (рестайлінг) (https://developers.ria.com/auto/new/generation_bodystyles?generation_id=432&api_key=YOUR_API_KEY), список типів кузова буде таким:

```javascript
[
  {
    "bodystyle_id":324,
    "eng":"krossover",
    "generation_bodystyle_id":538,
    "name":"Кросовер"
  }
]
```
