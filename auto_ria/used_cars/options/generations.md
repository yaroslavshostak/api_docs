## Покоління
Повертає список усіх поколінь авто для конкретної моделі авто.

**URL**
```
GET https://developers.ria.com/generations/by/models/modelID/generations?api_key=YOUR_API_KEY
```
де *modelId* - ідентифікатор моделі авто, *YOUR_API_KEY* - персональний ключ доступу користувача.

**Зразок запиту**
```
GET https://developers.ria.com/generations/by/models/1653/generations?api_key=YOUR_API_KEY
```

**Відповідь**

<table style="width:100%;">
<thead>
<tr>
<th style="text-align:center;">Параметр</th>
<th style="text-align:center;">Опис</th>
<th style="text-align:center;">Тип</th>
<th style="text-align:center;">Деталі</th>  
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">name</td>
<td style="text-align:left;">Назва моделі авто</td>
<td style="text-align:center;"><code>string</code></td>
<td style="text-align:center;"> </td>
</tr>
<tr>
<td style="text-align:left;">id</td>
<td style="text-align:left;">Ідентифікатор моделі авто</td>
<td style="text-align:center;"><code>integer</code></td>
<td style="text-align:center;"> </td>
</tr>
<tr>
<td style="text-align:left;">generations</td>
<td style="text-align:left;">Покоління авто</td>
<td style="text-align:center;"><code>array of generations data objects</code></td>
<td style="text-align:center;"> </td>
</tr>
<tr>
<td style="text-align:left;">generationId</td>
<td style="text-align:left;">Ідентифікатор покоління авто </td>
<td style="text-align:center;"><code>integer</code></td>
<td style="text-align:center;"> </td>
</tr>   
<tr>
<td style="text-align:left;">name</td>
<td style="text-align:left;">Назва покоління авто</td>
<td style="text-align:center;"><code>string</code></td>
<td style="text-align:center;"> </td>
</tr>      
<tr>
<td style="text-align:left;">yearFrom</td>
<td style="text-align:left;">Рік випуску авто - початкове значення</td>
<td style="text-align:center;"><code>integer</code></td>
<td style="text-align:center;"> </td>
</tr> 
<tr>
<td style="text-align:left;">yearTo</td>
<td style="text-align:left;">Рік випуску авто - кінцеве значення</td>
<td style="text-align:center;"><code>integer</code></td>
<td style="text-align:center;"> </td>
</tr>
<tr>
<td style="text-align:left;">modelID</td>
<td style="text-align:left;">Ідентифікатор моделі авто</td>
<td style="text-align:center;"><code>integer</code></td>
<td style="text-align:center;"> </td>
</tr>
<tr>
<td style="text-align:left;">eng</td>
<td style="text-align:left;">Сленгова назва покоління</td>
<td style="text-align:center;"><code>string</code></td>
<td style="text-align:center;">Латиниця</td>
</tr>
</tbody>
</table></div>
<br>  


**Зразок відповіді**
```
[
   {
      "name": "Caravelle",
      "id": 1653,
      "generations": [
         {
            "generationId": 16,
            "name": "III покоління (FL)/T5",
            "yearFrom": 2009,
            "yearTo": 2015,
            "modelId": 1653,
            "eng": "t5-fl"
         },
         {
            "generationId": 17,
            "name": "IV покоління/T6",
            "yearFrom": 2015,
            "yearTo": 2019,
            "modelId": 1653,
            "eng": "t6"
         },
         {
            "generationId": 8066,
            "name": "IV покоління (FL)/T6.1",
            "yearFrom": 2019,
            "yearTo": 0,
            "modelId": 1653,
            "eng": "t6-1"
         },
         {
            "generationId": 13684,
            "name": "I покоління/T3",
            "yearFrom": 1981,
            "yearTo": 1992,
            "modelId": 1653,
            "eng": "1-pokolenie"
         },
         {
            "generationId": 13686,
            "name": "II покоління/T4",
            "yearFrom": 1990,
            "yearTo": 1996,
            "modelId": 1653,
            "eng": "2-pokolenie"
         },
         {
            "generationId": 13688,
            "name": "II покоління (FL)/T4",
            "yearFrom": 1996,
            "yearTo": 2003,
            "modelId": 1653,
            "eng": "2-pokolenie-fl"
         },
         {
            "generationId": 13689,
            "name": "III покоління/T5",
            "yearFrom": 2003,
            "yearTo": 2009,
            "modelId": 1653,
            "eng": "3-pokolenie"
         }
      ]
   }
]
```
