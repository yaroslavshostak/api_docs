### Райони

 Райони залежать від міст, тому, щоб отримати їхній список, необхідно надіслати GET запит за адресою `https://developers.ria.com/dom/cities_districts/:city_id?api_key=YOUR_API_KEY`, де *city_id* - ідентифікатор міста.
  
Наприклад, для міста Львова ([https://developers.ria.com/dom/cities_districts/5?api_key=YOUR_API_KEY](https://developers.ria.com/dom/cities_districts/5?api_key=YOUR_API_KEY&) список районів буде таким:
  
  ```json
 [
[
{
"name": "Район",
"value": ""
},
{
"city_id": 5,
"area_id": 20169,
"name": "Батальна",
"type": 1,
"value": 20169
},
{
"city_id": 5,
"area_id": 17764,
"name": "Білогорща",
"type": 1,
"value": 17764
},
{
"city_id": 5,
"area_id": 17765,
"name": "Богданівка (Залізничний)",
"type": 1,
"value": 17765
},
{
"city_id": 5,
"area_id": 17781,
"name": "Богданівка (Франківський)",
"type": 1,
"value": 17781
},
{
"city_id": 5,
"area_id": 15771,
"name": "Боднарівка",
"type": 1,
"value": 15771
},
{
"city_id": 5,
"area_id": 17769,
"name": "Великі Кривчиці",
"type": 1,
"value": 17769
}
...
]
]
