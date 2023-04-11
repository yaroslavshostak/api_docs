## Модифікації

Повертає список усіх модифікацій авто для конкретного покоління.

**URL**
```
GET https://developers.ria.com/modifications/by/generation/:generationID/modifications?api_key=YOUR_API_KEY
```
де *generationId* - ідентифікатор покоління авто, *YOUR_API_KEY* - персональний ключ доступу користувача.


**Зразок запиту**
```
GET https://developers.ria.com/modifications/by/generation/17/modifications?api_key=YOUR_API_KEY
```

**Відповідь**

<table>
<thead>
<tr>
<th style="text-align:left;">Параметр</th>
<th style="text-align:left;">Опис</th>
<th style="text-align:center;">Тип</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">name</td>
<td style="text-align:left;">Назва модифікації авто</td>
<td style="text-align:center;"><code>string</code></td>
</tr>
<tr>
<td style="text-align:left;">value</td>
<td style="text-align:left;">Ідентифікатор модифікації</td>
<td style="text-align:center;"><code>integer</code></td>
</tr>
</tbody>
</table></div>
   

**Зразок відповіді**
```
[
   {
      "name": "2.0 BiTDI DSG (180 к.с.)",
      "value": 115538
   },
   {
      "name": "2.0 BiTDI DSG (180 к.с.) 4Motion",
      "value": 115539
   },
   {
      "name": "2.0 TDI DSG (102 к.с.)",
      "value": 121490
   },
   ...
   
]
```
