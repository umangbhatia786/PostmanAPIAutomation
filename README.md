# PostmanAPIAutomation
Automation collections bulit on Postman

Library API:
Base URI:  https://rahulshettyacademy.com

             (or)    http://216.10.245.166
 
1.	Method: POST
Add Book Complete URL - https://rahulshettyacademy.com/Library/Addbook.php

aisle value should be number only. Isbn should be unique to insert. So provide random isbn which makes unique
Input Payload: Json:
{

"name":"Learn Appium Automation with Java",
"isbn":"bcd",
"aisle":"227",
"author":"John foe"
}
 
Output Json 
{
   "Msg": "successfully added",
   "ID": "bcd227"
} 


 
 
1.	Resource : /Library/GetBook.php?AuthorName=somename        Method : GET 
 
Output Json:
Output the array of Json object books with all below details 
 
{
 
Name : “bookname”   ( String)
Isbn :  “A2fdsf”   (String)
Aisle : 32 (Integer)
 
}
 
 
1.	Resource: Library/GetBook.php?ID=3389      - Method : GET 
 
Output Json:
{
      "book_name": "Selenium automation using Java",
      "isbn": "a23hd738",
      "aisle": "1223"
   } 
 
1.	Resource :/Library/DeleteBook.php      Method : POST
 
Input Payload: Json:
{
 
"ID" : "a23h345122332"
 
} 
Output Response:
{

msg : book is successfully deleted”
 
}
![image](https://github.com/umangbhatia786/PostmanAPIAutomation/assets/20531028/278f4f16-baff-4b7a-84f0-bf998e0b18cf)
