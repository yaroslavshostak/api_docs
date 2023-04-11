## Модифікації

Повертає список усіх модифікацій авто для конкретного покоління.

**URL**
```
GET https://developers.ria.com/modifications/by/generation/:generationID/modifications?api_key=YOUR_API_KEY
```
де *generationId* - ідентифікатор покоління авто, *YOUR_API_KEY* - персональний ключ доступу користувача.


**Зразок запиту**
```
GET https://developers.ria.com/modifications/by/generation/17/modifications?api_key=YOUR_API_KEY
```

**Відповідь**

<table>
| Параметер  | Опис                    |Тип       |
| ----------| :----------------------: |:--------:|
| name      | Назва модифікації авто   | string    |
| value     | Ідентифікатор модифікації| integer  |
</table>

**Зразок відповіді**
```
[
   {
      "name": "2.0 BiTDI DSG (180 к.с.)",
      "value": 115538
   },
   {
      "name": "2.0 BiTDI DSG (180 к.с.) 4Motion",
      "value": 115539
   },
   {
      "name": "2.0 TDI DSG (102 к.с.)",
      "value": 121490
   },
   ...
   
]
```
