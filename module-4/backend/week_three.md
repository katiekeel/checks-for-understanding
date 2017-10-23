## Week Three - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. At a high level, what is Node?
* It's a system that allows you to run and test Javascript outside of the browser.  

2. What is Express? What is Express similar to in the Ruby world?
* Express is a lightweight library that allows you to define routes and return things from your server to display to a user, like Sinatra in Ruby.  

3. How do we setup a route when creating an API with Node and Express? Please provide a code snippet.

Where app is defined based on your configuration setup:  

`$ app.get('/api/v1/whatever)`

4. What do we use Knex for?  

Knex is a not-quite-an-ORM that helps us connect to our database in Node. (Like ActiveRecord, but worse.)  

5. How could you organize your code to follow the MVC design pattern in your Quantified Self project?  

Because Express isn't opinionated, you can set up models, controllers, and views folder just as you would in Rails.   

6. How do you execute raw SQL in node?  

You can use Knex's `database.raw('SQL statement')` method.  

7. What are some advantages to having your front end and back end code live in separate applications? What are some disadvantages?  

* Advantages: I, as a backend person, don't need to care about views. I just give the frontend people the data and that's that. They, as frontend people, don't need to worry about databases, writing API routes, or anything like that.
* Disadvantages: If you're a full stack developer, it takes more configuration to have two apps talk to one another than it does to have everything within the same app.

#### Review  

8. Describe DNS.  
* Domain Name System - the way that web browsers find and deliver the address you type into your search bar. It involves a series of servers, who all have different pieces of information related to the URI you've requested, telling your router how to find what you've asked for.

9. What does writing clean code mean to you?  
* No logic in the views, short methods, things broken out into classes, etc.

10. If you were building an application that models hotels, what classes would you need? What classes would be responsible for what functionality?  

At a minimum:

* Hotel class - initialized with x number of Rooms
* Room class - rooms belong to a hotel
* Guest class - guests belong to a room
