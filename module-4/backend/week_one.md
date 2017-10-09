## Week One - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. What's the most useful thing you learned from completing the intermission week work?  
* A reminder on how to write JS loops
2. What are some tools to help debug JavaScript code?  
* pryjs, debugger
3. What are some tools you need in order to unit test your JavaScript?  
* Mocha and Chai, installed with npm
4. What is the syntax for invoking a function?  
* Just call it by name with any params it might take:
```myFunction(arg);```
5. What's `this` in JavaScript?
* Similar to self in Ruby, refers to the object you're calling it on... sometimes
6. What is Webpack and why is it useful?
* It's like ```rake assets:precompile``` in Rails, but it works better and automatically
7. When/why do you want to use event delegation?
* It can be used to create events farther up the DOM than the one the user has performed an action on 
8. What's `npm` and what do we use it for?
* Node package manager; we use it similar to the way we would use the ```rails``` keyword. i.e. ```npm start``` instead of ```rails server```

#### Review  
9. What's the MVC design pattern? Describe each part of MVC.
* Model, view, controller - the controller routes requests to the server, the view renders what the user sees, and the model communicates with the database
10. What are a few ways to optimize a Rails application?
* Removing n+1 queries, caching, using background workers
11. What's a background worker? When would we want to use a background worker?
* It schedules tasks for the server (or multiple servers) to perform at different times in the future so that the immediate response to the user isn't slowed down by logical dependencies
