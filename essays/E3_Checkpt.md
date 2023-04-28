---
layout: essay
type: essay
title: "Checkpoint Assignment 3"
# All dates must be YYYY-MM-DD format!
date: 2023-04-27
published: true
labels:
  - Assignment 3
---

#### 1. Show what each page will look like. The pages do not have to be “functional” but the design should clear.

Click [here](https://youtu.be/y--ARHPIQQE) to watch a screencast where I present the design and functionality of my e-commerce website. 

#### 2. Describe your design for your site’s shopping cart. That is, will it be a separate page that the user can view and edit, or will it be integrated into the product pages? If so, describe in detail how this will work on your site. Provide several examples of using the cart.

I plan to have my shopping cart be on a separate page that the user can view and edit to their liking (adding or removing quantities). I thought that it would be nice to have a side bar shopping cart, so that users can just edit their quantities and shopping cart without being directed to another page, but I'm not confident about accomplishing this. If I feel that I have the time, I might challenge myself with making the shopping cart a side bar feature. I have a purchase button on the products display page at the moment, but I will probably change this to something like "add to cart." If the user selects valid quantities and is logged in, they will be sent to the shopping cart page. On the shopping cart page, there would be a "complete purchase" button and a "continue shopping" button. The "complete purchase" button would redirect the user to the invoice page where they can view what they purchased. 

#### 3. Explain specifically how you will use sessions to manage your shopping cart. In particular, what shopping cart data will be stored in the session, what data format will be used (NOT what data type, but the format like with the data format used for your registration data). Use code examples showing what data structures (such as arrays and their objects) you will use to manage the shopping cart data and how they will be used in a session.

I will use sessions to manage my shopping cart by storing cart information, such as the products selected and the selected quantities for each product in the session. I plan to have an array of product objects that each hold information about the specific product. An example of what this would look like is: `request.session['soda']=[{"name":"Mitsuya Cider", "price": 2, "qty_purchased":2}];`

#### 4. How will you avoid access to your application when the user has not logged in or registered? What are the particular security concerns you must address?

In Assignment 2, I prevented unauthorized access to the invoice by checking whether or not the user's email was in the query URL. I can also do this with cookies (like in the Lab 14 Cookies and Sessions Lab) by using an if statement to check if the cookies has the user's username. If it exists, then the user will proceed to the invoice, and if not, they will be directed to the login page. In this assignment, I will also have to log out a user after a period of inactivity for security purposes. 

#### 5. Upon a successful login, how do you provide personalization in your UI? Explain how you did or will do this (paste code if necessary)

Upon a successful login, I plan to provide personalization in my UI by changing the login tab on the nav bar to display the user's username. The user can click on this tab to log themselves out. I also have a user-personalized thank you message on the invoice page that addresses the user by their username. I plan to implement these personalization ideas through accessing my cookie and session data. 

#### 6. If you are working with partners, how will you split up the work in your team so that you are working in parallel as effectively as possible? That is, who is doing what and when?

I am not working with a partner. 

#### 7. How are you approaching Assignment 3 differently than Assignment 2?

With the Assignment 3 Extra Credit opportunity, I will be forced to list all of the tasks for this assignment in advance, which will help me stay organized and visualize what exactly I need to do. I did this midway of doing Assignment 2, which helped with my progress, so I hope that my journey to finishing Assignment 3 will be smoother than it was for Assignment 2. 
