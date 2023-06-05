# [](#Подсчёт-средней-цены)**Підрахунок середньої ціни**

**“Підрахунок середньої ціни”** — сервіс, заснований на актуальних статистичних даних **DIM.RIA**

Тепер ви можете:

*   дізнаватися актуальні середні ціни на нерухомість;

*   стежити за змінами цін у коротко- і довгостроковому періодах;

*   аналізувати та прогнозувати зміни цін і попиту на нерухомість;

*   розміщувати отриману інформацію на вашому сайті.

    Ознайомтеся з технічною документацією, щоб отримати доступ і експортувати необхідну інформацію в програму вашої компанії.


У разі успішного підрахунку середньої ціни за вказаними параметрами результат буде зі статусом **200 OK**.

### Формат даних у запиті

<table>

<thead>

<tr>

<th align="left">Назван</th>

<th align="left">Параметр у рядку запиту</th>

<th align="center">Тип даних</th>

</tr>

</thead>

<tbody>

<tr>

<td align="left">Тип об'єкта</td>

<td align="left">category</td>

<td align="center">`Number`</td>

</tr>

<tr>

<td align="left">Тип нерухомості</td>

<td align="left">sub_category</td>

<td align="center">`Number`</td>

</tr>

<tr>

<td align="left">Тип операції</td>

<td align="left">operation</td>

<td align="center">`Number`</td>

</tr>

<tr>

<td align="left">Область</td>

<td align="left">state_id</td>

<td align="center">`Number`</td>

</tr>

<tr>

<td align="left">Місо</td>

<td align="left">city_id</td>

<td align="center">`Number`</td>

</tr>

<tr>

<td align="left">Район</td>

<td align="left">district_id</td>

<td align="center">`Number`</td>

</tr>

<tr>

<td align="left">Дата видачі від</td>

<td align="left">date_from</td>

<td align="center">`Number`</td>

</tr>

<tr>

<td align="left">Дата видачі до</td>

<td align="left">date_to</td>

<td align="center">`Number`</td>

</tr>

</tbody>

</table>

Параметри **category**, **sub_category**, **operation** є обов'язковим для заповнення.


Приклад успішного запиту:
````javascript
  https://developers.ria.com/dom/average_price?category=1&sub_category=2&operation=1&state_id=1&city_id=1&date_from=2017-06&date_to=2017-07&api_key=YOUR API KEY
````
або
````javascript
    curl -X GET "https://developers.ria.com/dom/average_price?category=1&sub_category=2&operation=1&state_id=1&city_id=1&date_from=2017-06&date_to=2017-07&api_key=YOUR API KEY" -H "accept: application/json"
````
Приклад успішної відповіді:

    {
      "total": 12407,
      "arithmeticMean": 785340.3,
      "prices": [
        {
          "count": 229,
          "value": 60000
        },
        {
          "count": 234,
          "value": 160000
        },
        {
          "count": 239,
          "value": 260000
        },
        {
          "count": 243,
          "value": 360000
        },
        {
          "count": 247,
          "value": 460000
        },
        {
          "count": 250,
          "value": 560000
        },
        {
          "count": 252,
          "value": 660000
        },
        {
          "count": 254,
          "value": 760000
        },
        {
          "count": 255,
          "value": 860000
        },
        {
          "count": 255,
          "value": 960000
        },
        {
          "count": 255,
          "value": 1060000
        },
        {
          "count": 254,
          "value": 1160000
        },
        {
          "count": 252,
          "value": 1260000
        },
        {
          "count": 250,
          "value": 1360000
        },
        {
          "count": 247,
          "value": 1460000
        },
        {
          "count": 243,
          "value": 1560000
        },
        {
          "count": 239,
          "value": 1660000
        },
        {
          "count": 234,
          "value": 1760000
        },
        {
          "count": 229,
          "value": 1860000
        },
        {
          "count": 224,
          "value": 1960000
        },
        {
          "count": 217,
          "value": 2060000
        },
        {
          "count": 211,
          "value": 2160000
        },
        {
          "count": 204,
          "value": 2260000
        },
        {
          "count": 197,
          "value": 2360000
        },
        {
          "count": 189,
          "value": 2460000
        },
        {
          "count": 182,
          "value": 2560000
        },
        {
          "count": 174,
          "value": 2660000
        },
        {
          "count": 166,
          "value": 2760000
        },
        {
          "count": 158,
          "value": 2860000
        },
        {
          "count": 150,
          "value": 2960000
        },
        {
          "count": 142,
          "value": 3060000
        },
        {
          "count": 134,
          "value": 3160000
        },
        {
          "count": 126,
          "value": 3260000
        },
        {
          "count": 119,
          "value": 3360000
        },
        {
          "count": 111,
          "value": 3460000
        },
        {
          "count": 104,
          "value": 3560000
        },
        {
          "count": 97,
          "value": 3660000
        },
        {
          "count": 90,
          "value": 3760000
        },
        {
          "count": 83,
          "value": 3860000
        },
        {
          "count": 77,
          "value": 3960000
        },
        {
          "count": 71,
          "value": 4060000
        },
        {
          "count": 65,
          "value": 4160000
        },
        {
          "count": 60,
          "value": 4260000
        },
        {
          "count": 55,
          "value": 4360000
        },
        {
          "count": 50,
          "value": 4460000
        },
        {
          "count": 46,
          "value": 4560000
        },
        {
          "count": 41,
          "value": 4660000
        },
        {
          "count": 37,
          "value": 4760000
        },
        {
          "count": 34,
          "value": 4860000
        },
        {
          "count": 30,
          "value": 4960000
        },
        {
          "count": 27,
          "value": 5060000
        },
        {
          "count": 24,
          "value": 5160000
        },
        {
          "count": 22,
          "value": 5260000
        },
        {
          "count": 19,
          "value": 5360000
        },
        {
          "count": 17,
          "value": 5460000
        },
        {
          "count": 15,
          "value": 5560000
        },
        {
          "count": 14,
          "value": 5660000
        },
        {
          "count": 12,
          "value": 5760000
        },
        {
          "count": 10,
          "value": 5860000
        },
        {
          "count": 9,
          "value": 5960000
        },
        {
          "count": 8,
          "value": 6060000
        },
        {
          "count": 7,
          "value": 6160000
        },
        {
          "count": 6,
          "value": 6260000
        },
        {
          "count": 5,
          "value": 6360000
        },
        {
          "count": 5,
          "value": 6460000
        },
        {
          "count": 4,
          "value": 6560000
        },
        {
          "count": 3,
          "value": 6660000
        },
        {
          "count": 3,
          "value": 6760000
        },
        {
          "count": 2,
          "value": 6860000
        },
        {
          "count": 2,
          "value": 6960000
        },
        {
          "count": 2,
          "value": 7060000
        },
        {
          "count": 2,
          "value": 7160000
        },
        {
          "count": 1,
          "value": 7260000
        },
        {
          "count": 1,
          "value": 7360000
        },
        {
          "count": 1,
          "value": 7460000
        },
        {
          "count": 1,
          "value": 7560000
        },
        {
          "count": 1,
          "value": 7660000
        },
        {
          "count": 1,
          "value": 7760000
        }
      ]
    }

Розшифрування параметрів:

*   _total_ - загальна кількість оголошень, що беруть участь у підрахунку.
*   _arithmeticMean_ - [середнє арифметичне](https://ru.wikipedia.org/wiki/%D0%A1%D1%80%D0%B5%D0%B4%D0%BD%D0%B5%D0%B5_%D0%B0%D1%80%D0%B8%D1%84%D0%BC%D0%B5%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%BE%D0%B5).
*   _count_ - кількість оголошень
*   _value_ - ціна в доларах США
