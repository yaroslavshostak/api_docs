### Продаж/оренда гаражів

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

<table>
<thead>
                <tr>
                    <th style="text-align:left">Назва</th>
                    <th style="text-align:left">Параметр в рядку запиту</th>
                    <th style="text-align:center">Тип даних</th>
                </tr>
                </thead>
                <tbody>
                <tr>
                    <td style="text-align:left">Тип об'єкта</td>
                    <td style="text-align:left">category</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Тип нерухомості</td>
                    <td style="text-align:left">realty_type</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Тип операції</td>
                    <td style="text-align:left">operation_type</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Область</td>
                    <td style="text-align:left">state_id</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Місто</td>
                    <td style="text-align:left">city_id</td>
                    <td style="text-align:center"><code>Number[]</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Район</td>
                    <td style="text-align:left">district_id</td>
                    <td style="text-align:center"><code>Number[]</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Машиномісць</td>
                    <td style="text-align:left">characteristic[211][from] - characteristic[211][to]</td>
                    <td style="text-align:center"><code>Number[]</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Загальна</td>
                    <td style="text-align:left">characteristic[214][from] - characteristic[214][to]</td>
                    <td style="text-align:center"><code>Number[]</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Призначення</td>
                    <td style="text-align:left">characteristic[175]</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Ціна</td>
                    <td style="text-align:left">characteristic[234][from] - characteristic[234][to]</td>
                    <td style="text-align:center"><code>Number[]</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Ціна</td>
                    <td style="text-align:left">characteristic[235][from] - characteristic[235][to]</td>
                    <td style="text-align:center"><code>Number[]</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Ціна договірна</td>
                    <td style="text-align:left">characteristic[1011]</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Стартова ціна</td>
                    <td style="text-align:left">characteristic[1464]</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Тип валюти</td>
                    <td style="text-align:left">characteristic[242]</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Можливий обмін</td>
                    <td style="text-align:left">characteristic[265]</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Можливий торг</td>
                    <td style="text-align:left">characteristic[273]</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Можлива розстрочка/кредит</td>
                    <td style="text-align:left">characteristic[274]</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Тип пропозиції</td>
                    <td style="text-align:left">characteristic[1437]</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Тільки з картою</td>
                    <td style="text-align:left">with_map</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Тільки з відео</td>
                    <td style="text-align:left">with_video</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Тільки з фото</td>
                    <td style="text-align:left">with_photo</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Тільки з фото (більше 3 фото)</td>
                    <td style="text-align:left">photos_count_from</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Тільки ТОП</td>
                    <td style="text-align:left">urgent_only</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Заставне майно</td>
                    <td style="text-align:left">banks_only</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Вторинне житло</td>
                    <td style="text-align:left">secondary</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Первинне житло</td>
                    <td style="text-align:left">newbuildings</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Не показувати мої оголошення</td>
                    <td style="text-align:left">exclude_my</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Не показувати оголошення від агентств</td>
                    <td style="text-align:left">exclude_agencies</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Дата подачі</td>
                    <td style="text-align:left">date_from - date_to</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                <tr>
                    <td style="text-align:left">Сторінка</td>
                    <td style="text-align:left">page</td>
                    <td style="text-align:center"><code>Number</code></td>
                </tr>
                </tbody>
            </table>
