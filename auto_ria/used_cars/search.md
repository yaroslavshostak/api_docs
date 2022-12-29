# API Пошуку


Щоб звернутися до RIA API search, Вам необхідно виконати GET запит такого вигляду:

https://developers.ria.com/auto/search?api_key=YOUR_API_KEY&PARAMETERS

або `curl -i -g -X GET "https://developers.ria.com/auto/search?api_key=YOUR_API_KEY&PARAMETERS" '`

Він складається з:

 * **SEARCH** — назва методу API, до якого Ви хочете звернутися.

 * **API_KEY** — ключ доступу. Для отримання ключа доступу потрібно зареєструватися на платформі developers.ria.com 

 * **PARAMETERS** — вхідні параметри, послідовність пар name=value, розділених амперсандом. Список параметрів вказано [тут](#user-content-Список-параметров)
 

У відповідь на такий запит Ви отримаєте відповідь у форматі JSON:

```javascript
[
 {
  "additional_params": {
    "lang_id": 2,                                             // Російська мова
    "page": 0,                                                // Порядковий номер сторінки
    "view_type_id": 0,
    "target": "search",
    "section": "auto",                                        // Пошук по авто
    "catalog_name": "",
    "elastica": true,
    "nodejs": true
  },
  "result": {                                                // Результат пошуку
    "search_result": {
      "ids": [                                               // id оголошень
        ....
        ....
        ....
        
      ],
      "count": 11,                                          // Кількість id оголошень доступних за заданими параметрами
      "last_id": 0,
      "qs": {
        "fields": [
          "_id"
        ],
        "size": 50,                                         // Кількість id оголошень, що відображаються
        "from": 0,  
 ]
```

## Приклад

Припустимо, Ви шукаєте:

* Легкові машини                                            ``(category_id=1)``
* Кузов *Седан*,*Універсал*                                 `(bodystyle[0]=3&bodystyle[4]=2)`
* Японія                                                   `(brandOrigin[0]=276)`
    * Toyota                                               ` (marka_id[0]=79)`
    * Всі моделі                                            `(model_id[0]=0)`
    * Рік випуску від 2010 до 2017р.                        ` (s_yers[0]=2010&po_yers[0]=2017)`
* Німеччина                                                  `(brandOrigin[1]=392)`
    * Volkswagen                                            `(marka_id[1]=84)`
    * Всі моделі                                            `(model_id[1]=0)`
    * Рік випуску від 2012 до 2016р.                        `(s_yers[1]=2012&po_yers[1]=2016)`      
* Ціна від 1000 до 60000                                     `(price_ot=1000&price_do=60000)`
    * Ціна вказана в доларах США                           ` (currency=1)`
* Можливий торг                                             `(auctionPossible=1)`
* Область
    * Вінницька - пошук по всіх містах цієї області       ` (state[0]=1&city[0]=0)`
    * Житомирська - пошук по всіх містах цієї області     ` (state[1]=2&city[1]=0)`
    * Київська - пошук по всіх містах цієї області        ` (state[2]=10&city[2]=0)`
* Не відображати авто, які знаходяться не в Україні       ` (abroad=2)`
* Не відображати нерозмитнені авто                       ` (custom=1)`
* Гаражне зберігання                                         `(auto_options[477]=477)`
* Паливо
    * Бензин                                                `(type[0]=1)`
    * Дизель                                                `(type[1]=2)`
    * Газ/бензин                                            `(type[3]=4)`
    * Електро                                               `(type[5]:6)`
* КПП
    * Ручна / Механіка                                     `(gearbox[0]=1)`
    * Автомат                                               `(gearbox[1]=2)`
    * Типтронік                                             `(gearbox[2]=3)`
* Об'єм 1.4 - 3.2 л.                                        `(engineVolumeFrom=1.4&engineVolumeTo=3.2)`
* Потужність 90 - 250                                         `(powerFrom=90&powerTo=250)`
    * Одиниця виміру потужності - к.с.                      `(power_name=1)`
* Тільки з фото                                             `(with_photo=1)`

У підсумку ми отримуємо запит такого [типу]:

[https://developers.ria.com/auto/search?api_key=YOUR_API_KEY&category_id=1&bodystyle[0]=3&....](https://developers.ria.com/auto/search?api_key=YOUR_API_KEY&category_id=1&bodystyle[0]=3&bodystyle[4]=2&marka_id[0]=79&model_id[0]=0&s_yers[0]=2010&po_yers[0]=2017&marka_id[1]=84&model_id[1]=0&s_yers[1]=2012&po_yers[1]=2016&brandOrigin[0]=276&brandOrigin[1]=392&price_ot=1000&price_do=60000&currency=1&auctionPossible=1&state[0]=1&city[0]=0&state[1]=2&city[1]=0&state[2]=10&city[2]=0&abroad=2&custom=1&auto_options[477]=477&type[0]=1&type[1]=2&type[3]=4&type[7]=8&gearbox[0]=1&gearbox[1]=2&gearbox[2]=3&engineVolumeFrom=1.4&engineVolumeTo=3.2&powerFrom=90&powerTo=250&power_name=1&countpage=50&with_photo=1)


У разі успішного виконання запиту за вказаними параметрами результат буде зі статусом **200 OK**.

Приклад успішної відповіді:
```javascript
[
    {
   "additional_params": {
     "lang_id": 2,                                  // Російська мова
     "page": 0,                                     // Порядковий номер сторінки
     "view_type_id": 0,
     "target": "search",
     "section": "auto",                             // Пошук по авто
     "catalog_name": "",
     "elastica": true,
     "nodejs": true
   },
   "result": {                                      // Результат пошуку
     "search_result": {
       "ids": [
         "19519211",
         "19684763",
         "19493489",
         "19714833",
         "19393702",
         "19692238",                                // id оголошень
         "19574398",
         "18154136",
         "19391327",
         "18693600",
         "19431563",
         "18047892"
       ],
       "count": 1,                                 // Кількість id оголошень доступних за заданими параметрами
       "last_id": 0, 
       "qs": {
         "fields": [
           "_id"
         ],
         "size": 50,                                // Кількість відображуваних id оголошень
         "from": 0,
             } 
            }     
           }
   }   
 ]
```


**Важливо**

Максимальна кількість id оголошень, що відображаються, за один запит дорівнює 100(*countpage*).У разі якщо результат 
пошуку перевищує це значення можна додати параметр *page* (порядковий номер сторінки) за допомогою якого можна 
переглянути всі результати пошуку.

```
"additional_params": {
    "lang_id": 2,
    "page": "1",                           // Порядковий номер сторінки     
    "view_type_id": 0,
    "target": "search",
    "section": "auto",
    "catalog_name": "",
    "elastica": true,
    "nodejs": true
  },
  "result": {
    "search_result": {
      "ids": [
        "19885907",
        "19885290",
        "19847856",
        "19876230",
        "19662019",
        "18493054",
        "19440597",
        "19865852",
        "18814906",
        "19862470",
        "19738583",
       . . . . . . .     
        "19860637",
        "19747721",
        "18050784",
        "19810589",
        "19746765",
        "18412097",
        "18545537"
      ],
      "count": 1578,                         // Кількість id за результатами пошуку
      "last_id": 0,
      "qs": {
        "fields": [
          "_id"
        ],
        "size": 100,
        "from": 100,
```


