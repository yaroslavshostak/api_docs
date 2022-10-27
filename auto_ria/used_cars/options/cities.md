### Міста

Міста залежать від областей - тому, щоб отримати їх список, необхідно надіслати GET запит за адресою `https://developers.ria.com/auto/states/:stateId/cities?api_key=YOUR_API_KEY`, де *stateId* - ідентифікатор області, *api_key*- Ваш ключ.

Наприклад, для Вінницької області ([https://developers.ria.com/auto/states/1/cities?api_key=YOUR_API_KEY](https://developers.ria.com/auto/states/1/cities?api_key=YOUR_API_KEY)) список міст буде таким:
```javascript
[
    {"name":"Вінниця","value":1},
    {"name":"Жмеринка","value":27},
    {"name":"Козятин","value":30},
    {"name":"Крижопіль","value":31},
    {"name":"Липовець","value":32},
    {"name":"Літин","value":33},
    {"name":"Могилів-Подільський","value":34},
    {"name":"Муровані Курилівці","value":35},
    {"name":"Немирів","value":36},
    {"name":"Оратів","value":37},
    {"name":"Піщанка","value":38},
    {"name":"Погребище","value":39},
    {"name":"Теплик","value":40},
    {"name":"Тиврів","value":41},
    {"name":"Томашпіль","value":42},
    {"name":"Тростянець","value":43},
    {"name":"Тульчин","value":44},
    {"name":"Хмільник","value":45},
    {"name":"Чернівці","value":46},
    {"name":"Чечельник","value":47},
    {"name":"Шаргород","value":48},
    {"name":"Ямпіль","value":49},
    {"name":"Бар","value":597},
    {"name":"Бершадь","value":599},
    {"name":"Гайсин","value":602},
    {"name":"Іллінці","value":603},
    {"name":"Калинівка","value":604},
    {"name":"Гнівань","value":609},
    {"name":"Ладижин","value":644},
    {"name":"Якушинці","value":1595}
]
```
