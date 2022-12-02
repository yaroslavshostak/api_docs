### Додавання фото до оголошення

Для додавання фотографій до оголошення, Вам необхідно виконати POST запит такого типу:
````javascript
curl -X POST "https://developers.ria.com/auto/used/autos/advertisementId/photos/upload?user_id=Ваш ID&api_key=YOUR API KEY" -H "accept: application/json" -H "content-type: application/json" -d "{ \"main\": \"головне фото\", \"links\": [ \"фотографії" ]}"
````
Розшифрування параметрів:

- *advertisementId* - ID потрібного Вам оголошення
- *user_id* - Ваш ID у системі RIA.com
- *api_key* - Ваш ключ
- *`-d "{ \"main\": \"посилання на головну фотографію\", \"links\": [ \"посилання на фотографії" ]}"`* - тут Ви вказуєте масив фотографій, які хочете додати. У кожному посиланні на зображення має бути присутній формат

Фотографії будуть додані не за черговістю, а у випадковому порядку.

Повний опис сервісу "Додавання фотографій до оголошення" описаний за допомогою стандарту **DeFacto swagger 2.0** [тут](http://swagger.ria.com/ui/?api=auto/advertisements#/)

**Приклад запиту**
````javascript
curl -X POST "https://developers.ria.com/auto/used/autos/21739303/photos/upload?user_id=7069830&api_key=bVjbA3izvnu04o7Pliw41bXAlY3mIj03CfQpeMNC" -H "accept: application/json" -H "content-type: application/json" -d "{ \"main\": \"https://cdn0.riastatic.com/photosnew/auto/photo/bmw_320__213471725fx.jpg\", \"links\": [ \"https://cdn0.riastatic.com/photosnew/auto/photo/bmw_320__213471725fx.jpg\", \"https://cdn0.riastatic.com/photosnew/auto/photo/bmw_320__213471726fx.jpg\" ]}"
`````
**Приклад успішної відповіді**
````javascript
{"message":"Ok","errors":[]}
````
