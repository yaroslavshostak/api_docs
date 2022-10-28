### Додавання нового фільтра на обмін

Для додавання нового фільтра на обмін в оголошення, Вам необхідно виконати POST запит такого типу:
````javascript 
curl -X POST "https://developers.ria.com/auto/used/autos/advertisementId/exchangeFilter?user_id=Ваш ID&api_key=YOUR_API_KEY" -H "accept: application/json" -H "content-type: application/json" -d "{\ \}"
````
 де *user_id* - Ваш ID у системі RIA.com, *advertisementId* - ID потрібного Вам оголошення, *`-d "{ \  \  }`* - тут Ви вказуєте масив параметрів на обмін які хочете додати,  *api_key* - Ваш ключ.

**Приклад запиту**

````javascript
curl -X POST "https://developers.ria.com/auto/used/autos/20438832/exchangeFilter?user_id=7069830&api_key=YOUR_API_KEY" -H "accept: application/json" -H "content-type: application/json" -d "{ \"brand\": { \"id\": 5 }, \"model\": { \"id\": 32 }, \"category\": { \"id\": 1 }, \"body\": { \"id\": 3 }, \"year\": { \"gte\": 2008, \"lte\": 2012 }}"`
`````

**Приклад успішної відповіді:**

````json
{"message":"Ok","errors":[],"success":true}
````

Повний опис сервісу "Додавання нового фільтра на обмін" описаний за допомогою стандарту **DeFacto swagger 2.0** [тут](http://swagger.ria.com/ui/?api=auto/advertisements#/)
