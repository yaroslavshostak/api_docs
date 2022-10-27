### Типи приводу

Типи приводу також залежать від типу транспорту - тому, щоб отримати їхній список, необхідно надіслати GET запит за адресою `https://developers.ria.com/auto/categories/:categoryId/driverTypes?api_key=YOUR_API_KEY`, де *categoryId* - ідентифікатор типу транспорту, *api_key*- Ваш ключ.

Наприклад, список типів приводу для мотоциклів ([https://developers.ria.com/auto/categories/2/driverTypes?api_key=YOUR_API_KEY](https://developers.ria.com/auto/categories/2/driverTypes?api_key=YOUR_API_KEY))виглядає таким чином:
```javascript
[
    {"name":"Кардан","value":4},
    {"name":"Ремінь","value":5},
    {"name":"Ланцюг","value":6}
]
```
