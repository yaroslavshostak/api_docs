## Пошук оголошень

Щоб скористатись DOM.RIA API search, Вам необхідно виконати GET запит такого виду:

https://developers.ria.com/dom/search?api_key=YOUR_API_KEY&PARAMETERS

або `curl -X GET "https://developers.ria.com/dom/search?api_key=YOUR_API_KEY&PARAMETERS"`
`  -H "accept: application/json"`

Він складається з:

 * **SEARCH** — назва методу API, до якого Ви хочете звернутися.

 * **API_KEY** — ключ доступу. Для отримання ключа доступу потрібно зареєструватися на платформі developers.ria.com 

 * **PARAMETERS** — вхідні параметри, послідовність параметів name=value, розділених амперсандом. Список параметрів вказано вище.

На такий запит Ви отримаєте відповідь у форматі JSON:

```json
{
  "items": [                //id оголошень
    
  ],
  "count":                // кількість
}
```

Повний опис сервісу "Пошук оголошень" описаний за допомогою стандарту DeFacto swagger 2.0
* [Квартир](http://swagger.ria.com/ui/?api=dom/apartments)
* [Будинків](http://swagger.ria.com/ui/?api=dom/house#/)
* [Комерційної нерухомості](http://swagger.ria.com/ui/?api=dom/commercial)
* [Офісів](http://swagger.ria.com/ui/?api=dom/offices)
* [Земельних ділянок](http://swagger.ria.com/ui/?api=dom/land)
* [Гаражів](http://swagger.ria.com/ui/?api=dom/garages)


**Приклад**

Припустимо, Ви шукаєте:
* Об'єкт - Квартири
* Тип нерухомості - квартира
* Операція - продаж
* Область - Київська
* Місто - Київ
* Район
   * Оболонський
   * Печерський
   * Подільський
* Кількість кімнат від 1 до 3
* Загальна площа від 60 до 90
* Житлова площа від 30 до 50
* Кухня від 4 до 9
* Кухня від 3 до 7
* Рік побудови - не вказано
* Ціна від 20000 до 90000
* Ціна за об'єкт
* Тип валюти долари США
* Можливий торг
* Тип пропозиції - від посередника


В результаті ми отримуємо запит такого [типу]:

[https://developers.ria.com/auto/search?api_key=YOUR_API_KEY&category=1&realty_type=2&operation_type=1....](https://developers.ria.com/dom/search?category=1&realty_type=2&operation_type=1&state_id=10&city_id=10&district_id=15187&district_id=15189&district_id=15188&characteristic[209][from]=1&characteristic[209][to]=3&characteristic[214][from]=60&characteristic[214][to]=90&characteristic[216][from]=30&characteristic[216][to]=50&characteristic[218][from]=4&characteristic[218][to]=9&characteristic[227][from]=3&characteristic[227][to]=7&characteristic[443]=442&characteristic[234][from]=20000&characteristic[234][to]=90000&characteristic[242]=239&characteristic[273]=273&characteristic[1437]=1434&api_key=YOUR_API_KEY)

або 
````javascript
curl -X GET "https://developers.ria.com/dom/search?category=1&realty_type=2&operation_type=1&state_id=10&city_id=10&district_id=15187&district_id=15189&district_id=15188&characteristic[209][from]=1&characteristic[209][to]=3&
characteristic[214][from]=60&characteristic[214][to]=90&characteristic[216][from]=30&characteristic[216][to]=50&
characteristic[218][from]=4&characteristic[218][to]=9&characteristic[227][from]=3&characteristic[227][to]=7&
characteristic[443]=442&characteristic[234][from]=20000&characteristic[234][to]=90000&
characteristic[242]=239&characteristic[273]=273&characteristic[1437]=1434&
api_key=YOUR_API_KEY" -H "accept: application/json"
````
У разі успішного виконання запиту за вказаними параметрами результат буде зі статусом **200 OK**.

Приклад успішної відповіді:

```json
{
  "items": [
    13336044,
    14076392,
    13814523,
    14064249,
    13078930,
    13927706,
    13962022
  ],
  "count": 7
}
```
