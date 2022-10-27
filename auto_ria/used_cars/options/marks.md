### Марки

Марки залежать від типів транспорту. Тому для того, щоб отримати список марок необхідно надіслати GET запит за адресою `https://developers.ria.com/auto/categories/:categoryId/marks?api_key=YOUR_API_KEY`, де *categoryId* -  ідентифікатор типу транспорту, *api_key*- Ваш ключ.

Наприклад, для легкових автомобілів ([https://developers.ria.com/auto/categories/1/marks?api_key=YOUR_API_KEY](https://developers.ria.com/auto/categories/1/marks?api_key=YOUR_API_KEY)), результат буде таким:
```javascript
[
    { name: "Acura", value: 98 },
    { name: "Adler", value: 2396 },
    { name: "Aixam", value: 2 },
    { name: "Alfa Romeo", value: 3 },
    { name: "Alpine", value: 100 },
    { name: "Altamarea", value: 3988 },
    { name: "Aro", value: 101 },
    { name: "Artega", value: 3105 },
    { name: "Asia", value: 4 },
    { name: "Aston Martin", value: 5 },
    { name: "Audi", value: 6 },
    { name: "Austin", value: 7 },
    { name: "Autobianchi", value: 102 }
    ...
]
```
