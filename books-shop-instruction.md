# 🚀 Books shop project

## Task
The books shop owner asked you to create the online shop to buy book with delivery to user's home. He wants the user to be able to look through the books' catalog, see the description of a particular book, add a book to the bag, choose the appropriate date and address to deliver. 

## Technical requirements
Compatible browsers: **Google Chrome, Mozilla Firefox**. We primarily develop for Google Chrome. Then we check to see if Mozilla Firefox is breaking our styles.

It's **prohibited** to use CSS frameworks (bootstrap, foundation, etc.).  
It's **prohibited** to use JS frameworks (Angular, React, Vue, etc.).  
It's **prohibited** to use legacy libraries (jQuery, etc.).
It's **prohibited** to use up-to-date libraries with a set of helper functions (lodash). 

It's **allowed** to use icon fonts and CSS preprocessors (SCSS).

It's **recommended** to use [normalize.css](https://necolas.github.io/normalize.css/).

## Repository requirements
- Create a public repository named "book-shop" on your GitHub account.
- You should deploy your task using gh-pages or by any other means.
- The commit history should reflect the development process of the application. Commit names should match the [commit requirements](https://docs.rs.school/#/git-convention)

## Stages of task completion
**Week_1**: Layout of catalog page 
 * the page should be created through the JavaScript code. It means, you have html file without tags (if you need, you may add main or div as wrapper, not more).
 * all tags should be created in the js code. 
 * styles you should describe in the css file,but you should add css classes to created tags using JavaScript,
 * the delivery form should be implemented in the HTML file ( not thru the js code )

**Week_2**: Add interactive to the pages: 
 * add book to the bag by click on appropriate button or by drag the image of book to the bag (drag and drop). Both options should be implemented
 * show popup with book's description by click on Show more button
 * close popup by click on Close or cross button 
 * remove book from the bag by the appropriate button, 
 * validation of form fields should run after user left the field (blur), 
 * summarize the personal information when user clicks on Complete button
 
 * ❗ do not forget to submit link to deployed application for cross-check till the end of the deadline

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

### Examples of layout
Pay attention, it's just the example on how the elements placed. The design is fully **up to students**. The authors of **top-5** most interesting design according to the activists vote will receive additional **20 points**

#### 🔗 Example Deployed Link: <a href="https://bayanalex.github.io/rs-books-shop/">Click here</a>

### Note
The json with books information you will find by the [link](books.json).Copy it to your project. To read json data from the file you may use next code 
```javascript   
fetch('../books.json') //path to the file with json data
        .then(response => {
            return response.json();
        })
        .then(data => {
            console.log(data);
        });
```

How to work with files, asynchronous data and so on will be in the future modules
