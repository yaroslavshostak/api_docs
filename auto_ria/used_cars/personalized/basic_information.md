###  Отримання основної інформації про оголошення

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

Щоб отримати основну інформацію про оголошення, Вам необхідно виконати GET запит такого вигляду:

https://developers.ria.com/auto/used/autos/advertisementId?user_id=Ваш ID&api_key=YOUR_API_KEY

або 
````javascript
curl -X GET "https://developers.ria.com/auto/used/autos/advertisementId?user_id=Ваш ID&api_key=YOUR_API_KEY" -H "accept: application/json"
`````
де *user_id* - Ваш ID в системі RIA.com, *advertisementId* - ID потрібного Вам оголошення, *api_key* - Ваш ключ.

**Приклад запиту**
````javascript
curl -X GET "https://developers.ria.com/auto/used/autos/20445742?user_id=7069830&api_key=YOUR_API_KEY" -H "accept: application/json"
`````
**Приклад успішної відповіді:**

```json
{
  "_id": 20445742,
  "fuel": {
    "consumption": {
      "city": 10,
      "route": 6,
      "combine": 8
    },
    "id": 2
  },
  "brand": {
    "id": 5
  },
  "model": {
    "id": 963
  },
  "modification": "V12 AMG B-turbo",
  "body": {
    "id": 6
  },
  "doors": 2,
  "gearbox": {
    "id": 1
  },
  "color": {
    "id": 10,
    "metallic": true
  },
  "year": 2016,
  "mileage": 32,
  "price": {
    "value": 80000,
    "currency": {
      "id": 1
    }
  },
  "post": {
    "auctions": true,
    "exchanges": {
      "type": {
        "id": 1
      },
      "payment": {
        "id": 2
      }
    },
    "comments": {
      "allowed": true,
      "check": false
    }
  },
  "spareParts": false,
  "user": {
    "id": 7069830,
    "type": "private"
  },
  "dates": {
    "created": "2017-09-13T06:26:35.000Z",
    "updated": "0000-00-00 00:00:00",
    "expired": "0000-00-00 00:00:00",
    "sold": "0000-00-00 00:00:00"
  },
  "status": {
    "id": 1
  },
  "partner": {
    "id": 1
  },
  "ip": 8091,
  "description": {
    "ru": "Авто в идеальном состоянии, вложений не требует",
    "uk": "Авто в ідеальному стані, вкладень не потребує"
  },
  "region": {
    "id": 10
  },
  "city": {
    "id": 10
  },
  "moderated": true,
  "damage": false,
  "custom": false,
  "photos": {
      "main": {
        "id": 196054982
         }
       },
  "credit": false,
  "video": {
    "key": "lLEiT9PeHSg"
  },
  "categories": {
    "main": {
      "id": 1
    },
    "all": [
      {
        "id": 1
      }
    ]
  },
  "drive": {
    "id": 2
  },
  "VIN": "JKBVNCB164A66XXXX",
  "confiscated": false,
  "verified": {
    "serviceStation": false
  },
  "seats": 2,
  "power": {
    "hp": 585,
    "kW": 430.56
  },
  "engine": {
    "volume": {
      "cc": 3500,
      "liters": 3.5
    }
  }
}
```
