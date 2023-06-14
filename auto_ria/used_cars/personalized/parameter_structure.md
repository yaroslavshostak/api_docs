
### Структура параметрів


**Параметри, які повинні обов'язково бути присутніми в запиті**


<table>

<thead>

<tr>

<th align="left">Ім'я поля</th>

<th align="left">Тип</th>

<th align="left">Опис</th>

<th align="left">Приклад</th>

</tr>

</thead>

<tbody>

<tr>

<td align="left">* year</td>

<td align="left">number</td>

<td align="left">Рік випуску вашого авто</td>

<td align="left">2016</td>

</tr>

<tr>

<td align="left">* price</td>

<td align="left">object</td>

<td align="left">Ціна, по якій ви бажаєте продати ваше авто</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">value</td>

<td align="left">number</td>

<td align="left">Значення</td>

<td align="left">80000</td>

</tr>

<tr>

<td align="left">currency</td>

<td align="left">object</td>

<td align="left">Валюта в якій ви продаєте ваш автомобіль</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">id</td>

<td align="left">number</td>

<td align="left">ID валюти в якій ви продаєте ваш автомобіль</td>

<td align="left">1</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">*categories</td>

<td align="left">object</td>

<td align="left">Тип транспорту</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">main</td>

<td align="left">object</td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">id</td>

<td align="left">number</td>

<td align="left">ID типу транспорту</td>

<td align="left">1</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">* brand</td>

<td align="left">object</td>

<td align="left">Марка автомобіля</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">id</td>

<td align="left">number</td>

<td align="left">ID марки автомобіля</td>

<td align="left">5</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">* model</td>

<td align="left">object</td>

<td align="left">Модель автомобіля</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">id</td>

<td align="left">number</td>

<td align="left">ID моделі автомобіля</td>

<td align="left">963</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">modification</td>

<td align="left">string</td>

<td align="left">Назва модифікації вашого автомобіля</td>

<td align="left">V12 AMG B-turbo</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">*body</td>

<td align="left">object</td>

<td align="left">Тип кузова</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">id</td>

<td align="left">number</td>

<td align="left">ID типу кузова</td>

<td align="left">6</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">*mileage</td>

<td align="left">number</td>

<td align="left">Пробіг у тис.км.</td>

<td align="left">32</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">* region</td>

<td align="left">object</td>

<td align="left">Область у якій ви продаєте автомобіль</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">id</td>

<td align="left">number</td>

<td align="left">ID області в якій ви продаєте автомобіль</td>

<td align="left">10</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">* city</td>

<td align="left">object</td>

<td align="left">Місто в якому ви продаєте автомобіль</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">id</td>

<td align="left">number</td>

<td align="left">ID міста в якому ви продаєте автомобіль</td>

<td align="left">10</td>

</tr>

</tbody>

</table>

**Додаткові параметри**

<table>

<thead>

<tr>

<th align="left">Ім'я поля</th>

<th align="left">Тип</th>

<th align="left">Опис</th>

<th align="left">Приклад</th>

</tr>

</thead>

<tbody>

<tr>

<td align="left">damage</td>

<td align="left">boolean</td>

<td align="left">Ваше авто після ДТП</td>

<td align="left">false</td>

</tr>

<tr>

<td align="left">custom</td>

<td align="left">boolean</td>

<td align="left">Авто розмитнене</td>

<td align="left">false</td>

</tr>

<tr>

<td align="left">VIN</td>

<td align="left">string</td>

<td align="left">VIN код вашого автомобіля</td>

<td align="left">JKBVNCB164A6XXXX</td>

</tr>

<tr>

<td align="left">gearbox</td>

<td align="left">object</td>

<td align="left">Коробка передач</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">id</td>

<td align="left">number</td>

<td align="left">ID коробки передач</td>

<td align="left">1</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">drive</td>

<td align="left">object</td>

<td align="left">Тип приводу</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">id</td>

<td align="left">number</td>

<td align="left">ID типу приводу</td>

<td align="left">2</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">fuel</td>

<td align="left">object</td>

<td align="left">Тип палива</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">id</td>

<td align="left">number</td>

<td align="left">ID типу палива, яке підходить вашому автомобілю</td>

<td align="left">2</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">consumption</td>

<td align="left">object</td>

<td align="left">Витрата палива</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">route</td>

<td align="left">number</td>

<td align="left">Витрата палива по трасі</td>

<td align="left">6</td>

</tr>

<tr>

<td align="left">city</td>

<td align="left">number</td>

<td align="left">Витрата палива по місту</td>

<td align="left">10</td>

</tr>

<tr>

<td align="left">combine</td>

<td align="left">number</td>

<td align="left">Витрата палива в змішаному режимі</td>

<td align="left">8</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">engine</td>

<td align="left">object</td>

<td align="left">Об'єм двигуна</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">volume</td>

<td align="left">object</td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">liters</td>

<td align="left">number</td>

<td align="left">Об'єм двигуна в літрах</td>

<td align="left">3.5</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">power</td>

<td align="left">object</td>

<td align="left">Потужність вашого авто</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">hp</td>

<td align="left">number</td>

<td align="left">Потужність вашого авто в кінських силах</td>

<td align="left">585</td>

</tr>

<tr>

<td align="left">kW</td>

<td align="left">number</td>

<td align="left">Потужність вашого авто в кіловатах</td>

<td align="left">430</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">color</td>

<td align="left">object</td>

<td align="left">Колір</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">id</td>

<td align="left">number</td>

<td align="left">ID кольору вашого автомобіля</td>

<td align="left">10</td>

</tr>

<tr>

<td align="left">metallic</td>

<td align="left">boolean</td>

<td align="left">Колір металік</td>

<td align="left">true</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">post</td>

<td align="left">object</td>

<td align="left">Додати торг</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">auctions</td>

<td align="left">boolean</td>

<td align="left">Дозвіл додавати торги до вашого оголошення</td>

<td align="left">true</td>

</tr>

<tr>

<td align="left">comments</td>

<td align="left">object</td>

<td align="left">Коментар</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">allowed</td>

<td align="left">boolean</td>

<td align="left">Дозволи коментувати ваше оголошення</td>

<td align="left">true</td>

</tr>

<tr>

<td align="left">check</td>

<td align="left">boolean</td>

<td align="left">Чи потрібне ваше підтвердження під час додавання коментаря</td>

<td align="left">false</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">exchanges</td>

<td align="left">object</td>

<td align="left">Обмін</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">payment</td>

<td align="left">object</td>

<td align="left">Доплата</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">id</td>

<td align="left">number</td>

<td align="left">Варіанти доплати при додаванні обміну до вашого оголошення</td>

<td align="left">2</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">type</td>

<td align="left">object</td>

<td align="left">Тип обміну</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">id</td>

<td align="left">number</td>

<td align="left">ID типу обміну (на автомобіль, на нерухомість тощо)</td>

<td align="left">1</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">video</td>

<td align="left">object</td>

<td align="left">Відео</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">key</td>

<td align="left">string</td>

<td align="left">Ключ до відео на YouTube</td>

<td align="left">lLEiT9PeHSg</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">description</td>

<td align="left">object</td>

<td align="left">Опис</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">ru</td>

<td align="left">string</td>

<td align="left">Опис російською мовою</td>

<td align="left">"Авто в идеальном состоянии, вложений не требует"</td>

</tr>

<tr>

<td align="left">uk</td>

<td align="left">string</td>

<td align="left">Опис українською мовою</td>

<td align="left">"Авто в ідеальному стані, вкладень не потребує"</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">doors</td>

<td align="left">number</td>

<td align="left">Кількість дверей</td>

<td align="left">2</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">seats</td>

<td align="left">number</td>

<td align="left">Кількість сидячих місць</td>

<td align="left">2</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">country</td>

<td align="left">object</td>

<td align="left">Країна з якої був пригнаний автомобіль</td>

<td align="left"></td>

</tr>

<tr>

<td align="left">import</td>

<td align="left">object</td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">id</td>

<td align="left">number</td>

<td align="left">ID країни</td>

<td align="left">0</td>

</tr>

<tr>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

<td align="left"></td>

</tr>

<tr>

<td align="left">spareParts</td>

<td align="left">boolean</td>

<td align="left">Авто на запчастини</td>

<td align="left">false</td>

</tr>

</tbody>

</table> 



