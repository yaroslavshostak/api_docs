### Коробки передач

Коробки передач залежать від типу транспорту - тому, щоб отримати їх список необхідно надіслати GET запит за адресою `https://developers.ria.com/auto/categories/:categoryId/gearboxes?api_key=YOUR_API_KEY`, де *categoryId* - ідентифікатор типу транспорту, *api_key*- Ваш ключ .

Наприклад, список коробок передач для мотоциклів ([https://developers.ria.com/auto/categories/2/gearboxes?api_key=YOUR_API_KEY](https://developers.ria.com/auto/categories/2/gearboxes?api_key=YOUR_API_KEY)) буде виглядати наступним чином:
```javascript
[
    {"name":"Ручна / Механіка","value":1},
    {"name":"Автомат","value":2},
    {"name":"Типтронік","value":3},
    {"name":"Робот","value":4},
    {"name":"Варіатор","value":5}
]
```
