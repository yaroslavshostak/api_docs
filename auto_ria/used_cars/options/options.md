### Опції

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

Опції залежать від типу транспорту. Отримати їхній список можна надіславши GET запит за адресою `https://developers.ria.com/auto/categories/:categoryId/options?api_key=YOUR_API_KEY`, де *categoryId* - ідентифікатор типу транспорту, *api_key*- Ваш ключ.

Наприклад, список опцій для легкових автомобілів ([https://developers.ria.com/auto/categories/1/options?api_key=YOUR_API_KEY](https://developers.ria.com/auto/categories/1/options?api_key=YOUR_API_KEY)) матиме приблизно такий вигляд:
```javascript
[
   {"name":"Антиблокувальна система (ABS)","value":217},
   {"name":"Антипробуксовочна система (ASR)","value":606},
   {"name":"Блокування замків задніх дверей","value":622},
   {"name":"Броньований кузов","value":515},
   {"name":"Вибір режиму руху","value":610},
   {"name":"Датчик втоми водія","value":617},
   {"name":"Датчик проникнення в салон (датчик об`єму)","value":623},
   {"name":"Датчик тиску в шинах","value":620},
   {"name":"Допомога при спуску","value":611},
   {"name":"Допомога при старті в гору","value":609},
   {"name":"Запобігання зіткнення","value":612},
   {"name":"Іммобілайзер","value":604}
    ...
]
```
