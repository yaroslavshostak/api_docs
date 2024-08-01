# AUTO info  Інформація по id оголошення

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

Щоб звернутися до RIA API info, Вам необхідно виконати GET запит такого виду:

https://developers.ria.com/auto/info?api_key=YOUR_API_KEY&auto_id=**id_оголошення**

або 
 ````javascript
 curl -i -X GET "https://developers.ria.com/auto/info?api_key=YOUR_API_KEY&auto_id=id_оголошення"
````
Він складається з:

 * **info** — назва методу API, до якого Ви хочете звернутися.
 
 * **API_KEY** — ключ доступу. Для отримання ключа доступу потрібно зареєструватися на платформі developers.ria.com 

 * **auto_id=** — номер оголошення за яким потрібна інформація
 
## Приклад

Припустимо, Вам потрібна інформація по _19050985_ id.

Цей запит матиме такий вигляд:

https://developers.ria.com/auto/info?api_key=YOUR_API_KEY&auto_id=19050985

або  
````javascript
curl -i -X GET "https://developers.ria.com/auto/info?api_key=YOUR_API_KEY&auto_id=19050985"
````
В разі успішного виконання запиту результат буде зі статусом **200 OK**.

Приклад успішної відповіді:

```javascript
[
 {
  "userId": 489269,                                                                       // id користувача
  "chipsCount": 0,
  "locationCityName": "Дніпро",                                                           // Місто
  "auctionPossible": false,                                                               // Торг 
  "exchangePossible": false,                                                              // Обмін    
  "realtyExchange": false,                                                                // Обмін на нерухомість 
  "exchangeType": "Будь-який",                                                            // Тип обміна
  "exchangeTypeId": 0,                                                                    // Ідентифікатор типу обміну
  "addDate": "2017-04-24 23:02:06",                                                       // Дата і час додавання 
  "updateDate": "2017-04-24 23:02:06",                                                    // Дата і час оновлення 
  "expireDate": "2017-07-24 23:02:06",                                                    // Дата і час закінчення
  "userHideADSStatus": false,                                                             // Користувач приховав статус
  "userPhoneData": {
    "phoneId": "xxxxxxxxx",                                                               // id телефону користувача (дані не виводяться) 
    "phone": "(xxx) xxx xx xx"                                                            // Телефон користувача (дані не виводяться)
  },
  "USD": 33500,                                                                           // Вартість у доларах США
  "UAH": 880380,                                                                          // Вартість у гривнях
  "EUR": 30815,                                                                           // Вартість у євро
  "isAutoAddedByPartner": false,                                                          
  "partnerId": 0, 
  "levelData": {
    "level": 10,                                                                          // Рівень топа
    "label": 3,                                                                           // Мітка
    "hotType": "терміново",                                                               // Мітка "TOP" або "Терміново"
    "expireDate": "2017-05-04 23:02:07"                                                   // Дата і час закінчення мітки "TOP" "Терміново"
  },
  "autoData": {                                                                           // Характеристики автомобіля
    "description": "Отже. Настав час терміново продати свій улюблений автомобіль. " +
     "\r\nКупував його в серпні 2013 року. \Повністю обслужений на о",                    // Опис
    
    "version": "",
    "onModeration": false,
    "year": 2013,                                                                         // Рік випуску
    "autoId": 19050985,                                                                   // id оголошення
    "statusId": 0,                                                                        //  - 
    "withVideo": false,                                                                   // Наявність відео                               
    "race": "60 тыс. км",                                                                 // Пробіг
    "raceInt": 60,                                                                        // - 
    "fuelName": "Дизель",                                                                 // Тип палива
    "gearboxName": "Автомат",                                                             // Тип приводу
    "isSold": false,                                                                      // Цей параметр показує чи машину продано чи ні
    "mainCurrency": "USD",                                                                // Основна валюта
    "fromArchive": false,
    "categoryId": 1,                                                                      // Тип транспорту
    "custom": 0                                                                           
  },
  "markName": "Volvo",                                                                    // Марка автомобіля
  "markId": 85,                                                                           // id марки автомобіля
  "modelName": "XC90",                                                                    // Модель автомобіля
  "modelId": 824,                                                                         // id Моделі автомобіля
  "photoData": {                                                                          // Фото
    "count": 15,                                                                          // Кількість фотографій
    "seoLinkM": "https://cdn.riastatic.com/photosnew/auto/photo/volvo_xc90__181949196m.jpg",
    "seoLinkSX": "https://cdn.riastatic.com/photosnew/auto/photo/volvo_xc90__181949196sx.jpg",
    "seoLinkB": "https://cdn.riastatic.com/photosnew/auto/photo/volvo_xc90__181949196b.jpg",
    "seoLinkF": "https://cdn.riastatic.com/photosnew/auto/photo/volvo_xc90__181949196f.jpg"
  },
  "linkToView": "/auto_volvo_xc90_19050985.html",                                         // Посилання на оголошення
  "title": "Volvo XC90",                                                                  // Назва
  "stateData": {                                     
    "name": "Дніпро",                                                                     // Місто
    "regionName": "Дніпропетровська",                                                     // Область
    "linkToCatalog": "/city/dnepropetrovsk/",
    "title": "Пошук оголошень по місту Дніпро",
    "stateId": 11                                                                         // id Міста
  },
  "oldTop": {
    "isActive": true,
    "expireDate": ""
  },
  "canSetSpecificPhoneToAdvert": false,
  "dontComment": 0,
  "sendComments": 0,
  "badges": [
    
  ],
  "checkedVin": {                                                                       // Перевірка VIN-коду
    "isShow": false,                                                                    // Відображати VIN-код
    "linkToReport": "/vin-check/auto/19050985/",
    "hasRestrictions": false,                                                           // Обмеження
    "checkDate": "04.05.2017",
    "isChecked": false                                                                  //  VIN-код перевірено
  },
  "isLeasing": 0,   // Лізинг 
  "dealer": {
    "link": "",
    "logo": "",
    "type": "",
    "id": 0,
    "name": "",
    "packageId": 0,
    "typeId": 0
  },
  "withInfoBar": false,                                                                // Інформаційна панель
  "infoBarText": "",
  "optionStyles": [
    
  ]    
]
 ```  
