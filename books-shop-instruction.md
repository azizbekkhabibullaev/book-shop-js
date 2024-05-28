# 🚀 Books shop loyihasi

## Task
Kitoblar do'koni egasi sizdan foydalanuvchilar uydan chiqmagan holda kitob sotib olish uchun onlayn-do'kon yaratishingizni so'radi. U foydalanuvchidan kitoblar katalogini ko‘rib chiqish, ma’lum bir kitob haqida ma'lumot ko‘rish, savatga kitob qo‘shish, yetkazib berish uchun tegishli sanani va manzilni tanlash imkoniyatini berishini xohlaydi. 

#### 🔗 Shu linkka kirib ko'rishingiz mumkin: <a href="https://bayanalex.github.io/rs-books-shop/">Meni bosing!!!</a>

## Texnik talablari
Mos keladigan brauzerlar: **Google Chrome, Mozilla Firefox**. Biz birinchi navbatda Google Chrome uchun dasturni ishlab chiqamiz. Keyin biz Mozilla Firefox da bizning style larimiz buzilyaptimi yoki yo'qligini tekshiramiz.

CSS kutubxonalaridan (bootstrap, Foundation va boshqalar) foydalanish **taqiqlangan**.  
JS kutubxona/frameworklaridan (Angular, React, Vue va boshqalar) foydalanish **taqiqlangan**.  
Eski kutubxonalardan (jQuery va boshqalar) foydalanish **taqiqlangan**.
Yordamchi funksiyalar to‘plamiga (lodash) ega zamonaviy kutubxonalardan foydalanish **taqiqlangan**.

icon fonts va CSS protsessorlaridan (SCSS) foydalanishga **ruxsat berilgan**.

[normalize.css](https://necolas.github.io/normalize.css/) dan foydalanish **tavsiya etiladi**.

## Repository talablari
- GitHub akkauntingizda "book-shop" nomli public repository yarating.
- Siz o'z loyihangizni gh-pages yoki boshqa ma'noda joylashtirishingiz mumkin.
- Commit history ilovani ishlab chiqish jarayonini aks ettirishi kerak.

## 💯 Agar ingliz tilini biladigan bo'lsangiz to'liq quyidagi talablarda loyihani bajaring! Agar inglzi tilini bilmasangiz, faqatgina berilgan deploy linkka kirib, berilgan misolni bajarishingiz kifoya.
### Scoring criteria (maximum 100 points)
1. The content of catalog page created thru the JavaScript. User sees the book image, title, author, price, show more and add to bag buttons **+10**
2. After user clicks on Show more button the popup with description and close button are shown **10**
3. The HTML elements should be added to the page using document fragment **+10**
4. When the user adds the book to the bag (either by click on Add to bag button or by drag-and-drop), the book appears in the bag with shorten data (title, author, price) and remove (cross) button. Also, the total sum is updated **+20**
5. When user click on Confirm order he appears in the Order page ( with form )  **+5**
6. The order form contains fields with own validation rules and Complete button **+20**
   * Name (mandatory, the length not less than 4 symbols, strings only, without spaces)
   * Surname (mandatory, the length not less than 5 symbols, strings only, without spaces)
   * Delivery date(mandatory, not earlier than next day)
   * Street (mandatory, the length not less than 5 symbols, the numbers are allowed)
   * House number(mandatory, numbers only, positive numbers only)
   * Flat number(mandatory, numbers only, positive numbers only, the dash symbol is allowed. Means, the flat number shouldn't start with minus/dash symbol. For example:  -37 is invalid, but 1-37 is valid)
   * Choose the payment type(radio buttons group): Cash or Card (mandatory)
   * Choose 2 gifts:  (optional)
     - pack as a gift, 
     - add postcard, 
     - provide 2% discount to the next time, 
     - branded pen or pencil
7. The Complete button is disabled until the user full form with valid information **+5**
8. If user left the field empty or fill with invalid data, this field became red (means red border) and the validation message (The field is invalid)  is appeared. After user fix data and left the field again, the validation red border and message should disappear. **+5**
9. After user fill all mandatory field with valid information, the Complete button become active. **+10**
10. After user click on Complete button, he will see the summarized information: for instance, The order created. The delivery address is Amazing street house 3 flat 10. Customer John Gald. **5**

### Dizayn qoidalari
E'tiborli bo'ling, bu misol faqat elementlarning qanday joylashtirilganiga misol. Dizayn to'liq **talabalar ixtiyorida**.

#### 🔗 Shu linkka kirib ko'rishingiz mumkin: <a href="https://bayanalex.github.io/rs-books-shop/">Meni bosing!!!</a>

### Eslatma
Kitoblar maʼlumotlari bilan jsonni [link](books.json) orqali topasiz. Uni loyihangizga nusxalang. Fayldan json ma'lumotlarini o'qish uchun quyidagi koddan foydalanishingiz mumkin
```javascript   
fetch('../books.json') //path to the file with json data
        .then(response => {
            return response.json();
        })
        .then(data => {
            console.log(data);
        });
```
