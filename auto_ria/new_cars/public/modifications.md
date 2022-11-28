## Модифікації (бази) за типом кузова в поколінні
    
Модифікація (бази) залежить від типу кузова в поколінні. Отримати цей список можна надіславши GET запит за адресою `https://developers.ria.com/auto/new/generation_bodystyles_bases?generation_bodystyle_id=id&api_key=YOUR_API_KEY` , де *generation_bodystyle_id* - id типів кузова, *api_key*- Ваш ключ.

Наприклад, для моделі BMW X6 у поколінні E71 (рестайлінг) (https://developers.ria.com/auto/new/generation_bodystyles_bases?generation_bodystyle_id=538&api_key=YOUR_API_KEY), список модифікацій буде таким:

```javascript
[
 {
   "base_id":9036,
   "generation_bodystyle_id":538,
   "marka_id":9,
   "model_id":2153,
   "name":"50i Steptronic (407 к.с.) xDrive"
 },
 {
   "base_id":15821,
   "generation_bodystyle_id":538,
   "marka_id":9,
   "model_id":2153,
   "name":"40d Steptronic (306 к.с.) xDrive"
 },
 {
   "base_id":166827,
   "generation_bodystyle_id":538,
   "marka_id":9,
   "model_id":2153,
   "name":"30d Steptronic (245 к.с.) xDrive"
 }
]
```
