### Типи кузова

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

Типи кузова залежать від типів транспорту. Тому для того, щоб отримати список типів кузова, необхідно надіслати GET запит на адресу `https://developers.ria.com/auto/categories/:categoryId/bodystyles?api_key=YOUR_API_KEY`, де *categoryId* - ідентифікатор типу транспорту, *api_key*- Ваш ключ.

Наприклад, для легкових автомобілів ([https://developers.ria.com/auto/categories/1/bodystyles?api_key=YOUR_API_KEY](https://developers.ria.com/auto/categories/1/bodystyles?api_key=YOUR_API_KEY)),  результат буде наступним:
```javascript
[
    {"name":"Седан","value":3,"parentId":0},
    {"name":"Позашляховик / Кросовер","value":5,"parentId":0},
    {"name":"Мінівен","value":8,"parentId":0},
    {"name":"Мікровен","value":449,"parentId":0},
    {"name":"Хетчбек","value":4,"parentId":0},
    {"name":"Унiверсал","value":2,"parentId":0},
    {"name":"Купе","value":6,"parentId":0},
    {"name":"Кабріолет","value":7,"parentId":0},
    {"name":"Пікап","value":9,"parentId":0},
    {"name":"Ліфтбек","value":307,"parentId":0},
    {"name":"Фастбек","value":448,"parentId":0},
    {"name":"Лімузин","value":252,"parentId":0},
    {"name":"Родстер","value":315,"parentId":0}
]
```

Також типи кузова можуть бути розділені на групи. Це актуально для спецтехніки. Тому існує спосіб отримати згруповані типи кузова надіславши GET запит за адресою `https://developers.ria.com/auto/categories/:categoryId/bodystyles/_group?api_key=YOUR_API_KEY`, де *categoryId* - ідентифікатор типу транспорту, *api_key*- Ваш ключ.

Наприклад, для мотоциклів ([https://developers.ria.com/auto/categories/2/bodystyles/_group?api_key=YOUR_API_KEY](https://developers.ria.com/auto/categories/2/bodystyles/_group?api_key=YOUR_API_KEY)), результат буде наступним:
```javascript
[
    [
       {"name":"Інше","value":56,"parentId":0},
       {"name":"Вантажні моторолери, мотоцикли, скутери, мопеди","value":429,"parentId":56}
    ],
    [
       {"name":"Квадроцикли","value":35,"parentId":0},
       {"name":"Всюдихід-амфібія","value":43,"parentId":35},
       {"name":"Гольф-кар","value":44,"parentId":35},
       {"name":"Картинг","value":45,"parentId":35},
       {"name":"Квадроцикл дитячий","value":36,"parentId":35},
       {"name":"Квадроцикл спортивний","value":39,"parentId":35},
       {"name":"Квадроцикл утилітарний","value":41,"parentId":35},
       {"name":"Мотовсюдиход","value":42,"parentId":35}
    ],
    [
       {"name":"Міні мотоцикли","value":31,"parentId":0},
       {"name":"Міні крос (Пітбайк)","value":33,"parentId":31},
       {"name":"Міні спорт","value":32,"parentId":31}
    ],
    [
       {"name":"Мопеди","value":58,"parentId":0},
       {"name":"Максі-скутер","value":12,"parentId":58},
       {"name":"Мокик","value":427,"parentId":58},
       {"name":"Скутер / Мотороллер","value":11,"parentId":58},
       {"name":"Скутер для інвалідів","value":426,"parentId":58},
       {"name":"Скутер ретро","value":425,"parentId":58},
       {"name":"Скутери з кабіною","value":430,"parentId":58}
    ],
    [
       {"name":"Мотоцикли","value":13,"parentId":0},
       {"name":"Боббер","value":421,"parentId":13},
       {"name":"Кафе рейсер","value":423,"parentId":13},
       {"name":"Мотоцикл Багатоцільовий (All-round)","value":25,"parentId":13},
       {"name":"Мотоцикл Без обтікачів (Naked bike)","value":15,"parentId":13},
       {"name":"Мотоцикл з коляскою","value":29,"parentId":13},
       {"name":"Мотоцикл Кастом","value":30,"parentId":13},
       {"name":"Мотоцикл Классік","value":14,"parentId":13},
       {"name":"Мотоцикл Кросс","value":19,"parentId":13},
       {"name":"Мотоцикл Круізер","value":24,"parentId":13},
       {"name":"Мотоцикл Позашляховий (Enduro)","value":21,"parentId":13},
       {"name":"Мотоцикл Спорт-туризм","value":17,"parentId":13},
       {"name":"Мотоцикл Супермото (Motard)","value":22,"parentId":13},
       {"name":"Мотоцикл Тріал","value":20,"parentId":13},
       {"name":"Мотоцикл Туризм","value":16,"parentId":13},
       {"name":"Мотоцикл Чоппер","value":23,"parentId":13},
       {"name":"Скремблер","value":422,"parentId":13},
       {"name":"Спортбайк","value":18,"parentId":13}
     ],
     [
       {"name":"Снігохід","value":46,"parentId":0},
       {"name":"Гірські снігоходи","value":434,"parentId":46},
       {"name":"Міні-розбірні снігоходи","value":432,"parentId":46},
       {"name":"Мотобуксир","value":424,"parentId":46},
       {"name":"Снігомопеди та снігоскутери","value":436,"parentId":46},
       {"name":"Снігоходи для пполювання та рибалки","value":433,"parentId":46},
       {"name":"Спортивні снігоходи","value":435,"parentId":46},
       {"name":"Утилітарні снігоходи","value":431,"parentId":46}
     ],
       {"name":"Трайк","value":57,"parentId":0},
     [
       {"name":"Трицикл","value":34,"parentId":0},
       {"name":"Вантажні трицикли","value":428,"parentId":34}
     ]
```

Формат даних при цьому відрізняється від звичайного - це колекція об'єктів у якій є інші колекції. Група типів кузовів завжди починається з її назви. Наприклад, у групу *Квадроцикли* входять типи кузовів *Квадроцикл дитячий*, *Квадроцикл спортивний*, *Квадроцикл утилітарний*, *Мотовсюдихід* тощо.

Також, за необхідності, можна отримати просто весь список типів кузовів, надіславши GET запит за адресою [https://developers.ria.com/auto/bodystyles?api_key=YOUR_API_KEY](https://developers.ria.com/auto/bodystyles?api_key=YOUR_API_KEY).
