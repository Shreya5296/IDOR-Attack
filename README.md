# IDOR-Attack

It is relatively a very simple hacking technique that is used to fetch unauthorized data. 

Example to explain the concept-
Let’s login into the website!
https://networking-ecommerce-new.onrender.com/

For simplicity, we can use the following credentials - 
Email - john.doe@gmail.com
Password - hello_john

Okay, now let’s scroll down a little, and click on the “Buy Now!” button on any of the products!
We could see that the end of the URL has a URL parameter, id with some value.
Let’s try and change the value of this field
On changing the id value, the product changed!

This page gets to know which product the user wants to buy through the URL. It simply takes the product based on the ID that is mentioned.
This is known as an Insecure Direct Object Reference (IDOR). 
This vulnerability occurs when any application uses user-supplied information to access objects directly, without validating it.
For example, here, we wanted to buy a different product, but just by changing the URL, the product displayed to us becomes different, and if we place an order now, we can actually place the order on the new product instead of the one we wanted to buy earlier.

There could be sensitive data in the profile page, such as passwords, or payment details, etc.
By this design, anyone can access other user’s data through tweaking the URL, and this is a demonstration of an IDOR vulnerability.
