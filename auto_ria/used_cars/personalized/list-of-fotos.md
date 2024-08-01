### Отримання списку фотографій оголошення

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

Для отримання списку фотографій оголошення, Вам необхідно виконати GET запит такого типу:

'https://developers.ria.com/auto/fotos/advertisementId?api_key=YOUR_API_KEY'

де  *advertisementId* - ID потрібного Вам оголошення, *api_key* - Ваш ключ.

**Приклад запиту**
````javascript
https://developers.ria.com/auto/fotos/19860101?api_key=YOUR_API_KEY'
````
**Приклад успішної відповіді:**

````json
{
  "status": 1,
  "data": {
    "19860101": {
      "187203123": {
        "photo_id": 187203123,
        "auto_id": 19860101,
        "status": 0,
        "checked": 1,
        "standard": 0,
        "date_add": "2017-06-04 13:27:33",
        "description": null,
        "url": "auto/photo/18720/1872031/187203123/187203123.jpg",
        "formats": [
          "https://cdn.riastatic.com/photos/auto/photo/18720/1872031/187203123/187203123f.jpg",
          "https://cdn.riastatic.com/photos/auto/photo/18720/1872031/187203123/187203123fx.jpg"
        ]
      },
      "187203127": {
        "photo_id": 187203127,
        "auto_id": 19860101,
        "status": 0,
        "checked": 1,
        "standard": 0,
        "date_add": "2017-06-04 13:27:35",
        "description": null,
        "url": "auto/photo/18720/1872031/187203127/187203127.jpg",
        "formats": [
          "https://cdn.riastatic.com/photos/auto/photo/18720/1872031/187203127/187203127f.jpg",
          "https://cdn.riastatic.com/photos/auto/photo/18720/1872031/187203127/187203127fx.jpg"
        ]
      },
      "187203129": {
        "photo_id": 187203129,
        "auto_id": 19860101,
        "status": 0,
        "checked": 1,
        "standard": 0,
        "date_add": "2017-06-04 13:27:37",
        "description": null,
        "url": "auto/photo/18720/1872031/187203129/187203129.jpg",
        "formats": [
          "https://cdn.riastatic.com/photos/auto/photo/18720/1872031/187203129/187203129f.jpg",
          "https://cdn.riastatic.com/photos/auto/photo/18720/1872031/187203129/187203129fx.jpg"
        ]
      },
      "187203135": {
        "photo_id": 187203135,
        "auto_id": 19860101,
        "status": 0,
        "checked": 1,
        "standard": 0,
        "date_add": "2017-06-04 13:27:39",
        "description": null,
        "url": "auto/photo/18720/1872031/187203135/187203135.jpg",
        "formats": [
          "https://cdn.riastatic.com/photos/auto/photo/18720/1872031/187203135/187203135f.jpg",
          "https://cdn.riastatic.com/photos/auto/photo/18720/1872031/187203135/187203135fx.jpg"
        ]
      },
      "187203138": {
        "photo_id": 187203138,
        "auto_id": 19860101,
        "status": 0,
        "checked": 1,
        "standard": 0,
        "date_add": "2017-06-04 13:27:40",
        "description": null,
        "url": "auto/photo/18720/1872031/187203138/187203138.jpg",
        "formats": [
          "https://cdn.riastatic.com/photos/auto/photo/18720/1872031/187203138/187203138f.jpg",
          "https://cdn.riastatic.com/photos/auto/photo/18720/1872031/187203138/187203138fx.jpg"
        ]
      }
    }
  }
}
````
