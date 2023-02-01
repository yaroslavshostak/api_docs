#### Зміна статусу замовлення

Щоб змінити статус замовлення, потрібно надіслати PUT запит на адресу
````javascript
curl -X PUT "https://developers.ria.com/ria/basket/orders?user_id=*id*&order_id=*id*&api_key=YOUR_API_KEY" -H "accept: application/json" -H "content-type: application/json"
 -d "{ \"status\": 0}"
 `````
 , де *user_id* - id користувача, *order_id* - id замовлення, *status_id* - id статусу замовлення, 

 
 
 Відповідь буде наступною:
```javascript
{
  "status": true
}
```
