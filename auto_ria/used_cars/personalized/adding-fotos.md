### Додавання фото до оголошення

Для додавання фотографій до оголошення, Вам необхідно виконати POST запит такого типу:
````javascript
curl -X POST "https://developers.ria.com/auto/used/autos/ID_оголошення/photos/upload?user_id=ВАШ_ID&api_key=ВАШ_API_КЛЮЧ" -H "accept: application/json" -H "content-type: application/json" -H 'Cookie: PSP_ID=ВАШ_PSP_ID' -d '{ "main": "головне фото", "links": [ "фотографії" ]}'
````
Розшифрування параметрів:

- *advertisementId* - ID потрібного Вам оголошення
- *user_id* - Ваш ID у системі RIA.com
- *api_key* - Ваш ключ
- *`-d '{ "main": "посилання на головну фотографію\", "links": [ "посилання на фотографії" ]}'`* - тут Ви вказуєте масив фотографій, які хочете додати. У кожному посиланні на зображення має бути присутній формат

Фотографії будуть додані не за черговістю, а у випадковому порядку.

*Зверніть увагу!* Розмір фото не має перевищувати 25МБ

Детальніше про PSP_ID [тут](https://www.ria.com/uk/offert/cookie/#soglashenieHead4/).


**Приклад запиту**
````javascript
curl --location --request POST 'https://developers.ria.com/auto/used/autos/ID_оголошення/photos/upload?user_id=ВАШ_ID&api_key=ВАШ_API_КЛЮЧ' \
--header 'Content-Type: application/json' \
--header 'Cookie: PSP_ID=ВАШ_PSP_ID' \
--data-raw '{ "main": "https://cdn0.riastatic.com/photosnew/auto/photo/bmw_320__213471725fx.jpg", "links": [ "https://cdn0.riastatic.com/photosnew/auto/photo/bmw_320__213471725fx.jpg", "https://cdn0.riastatic.com/photosnew/auto/photo/bmw_320__213471726fx.jpg" ]}'
`````


**Приклад успішної відповіді**
````javascript
{"message":"Ok","errors":[]}
````
