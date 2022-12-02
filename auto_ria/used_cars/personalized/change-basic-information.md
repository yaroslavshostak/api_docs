### Зміна основної інформації оголошення

Для зміни основної інформації оголошення, Вам необхідно відправити **PUT** запит такого типу:
````javascript
curl -X PUT "https://developers.ria.com/auto/used/autos/advertisementId?user_id=Ваш ID&api_key=YOUR_API_KEY" -H "accept: application/json" -H "content-type: application/json"  -d "{ \  \  }
````
де *user_id* - Ваш ID в системі RIA.com, *advertisementId* - ID потрібного Вам оголошення, *`-d "{ \  \  }`* - тут Ви вказуєте масив параметрів які хочете змінити,  *api_key* - Ваш ключ.

 Детально з параметрами і структурою можна ознайомитися [тут](#user-content-Структура-параметров)

**Приклад запиту**

Припустимо, Вам потрібно змінити ціну і валюту, в якій ви продаєте ваш автомобіль. Цей запит матиме такий вигляд:
````javascript
curl -X PUT "https://developers.ria.com/auto/used/autos/20438832?user_id=7069830&api_key=YOUR_API_KEY" -H "accept: application/json" -H "content-type: application/json" -d "{ \"price\": { \"value\":10000, \"currency\": { \"id\":1 } }}"
`````
или изменить главное фото объявления, данный запрос будет иметь следующий вид:
````javascript
curl -X PUT "https://developers.ria.com/auto/used/autos/20438832?user_id=7069830&api_key=YOUR_API_KEY" -H "accept: application/json" -H "content-type: application/json" -d "{  \"photos\": { \"main\": { \"id\": 16652206 } }}"
`````
Об'єкт *price* містить у собі параметри *value* - значення, *currency* - ID валюти, в якій ви продаєте ваш автомобіль, у нашому випадку це долар.

**Приклад успішної відповіді:**
```json
{"message":"Ok",

"errors":[],

"success":true}
```

 Повний опис сервісу "Зміна основної інформації оголошення" описаний за допомогою стандарту **DeFacto swagger 2.0** [тут](http://swagger.ria.com/ui/?api=auto/advertisements#/)


**Важливо**

Основні параметри транспортного засобу доступні до редагування протягом години, після додавання на сайт:

 - “Регіон”

 - “Тип транспорту", "Марка", "Модель", "Версія", "Рік випуску”

 - “VIN-номер”, “Коробка передач”, “Привід", "Кількість дверей", "Колір", "Паливо”

Решту параметрів - "Ціна", "Пробіг", "Фото" автомобіля, докладний опис - можете змінювати і коригувати в будь-який час.

Якщо ж після закінчення 60 хв. відправити запит на зміну одного з вище перерахованих параметрів, Ви отримаєте помилку.

**Приклад помилки**

```json
{
   "message":"StatusCodeError: 400 - {\"message\":\"Validation failed\",\"errors\":[{\"message\":\"You can edit categories.main.id for 60 minutes\",\"code\":7},{\"message\":\"You can edit brand.id for 60 minutes\",\"code\":7},{\"message\":\"You can edit model.id for 60 minutes\",\"code\":7}]}"
}
```
