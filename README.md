# Testing TODOs with Mocha/Chai Lab

This is Part 3.1 (optional) of a series of labs working towards building your first full stack web app.

- [Part 1 - TDD todo list](https://github.com/wdi-sg/tdd-todo-list)
- [Part 2 - Mongo todo list](https://github.com/wdi-sg/mongo-todo-list)
- [Part 3 - Express todo list pt1](https://github.com/wdi-sg/express-todo-list-pt1)
- Part 3.1 - (this repo, which is optional)
- [Part 4 - Express todo list pt2](https://github.com/wdi-sg/express-todo-list-pt2)
- [Part 5 - Multi Model todo list](https://github.com/wdi-sg/multi-model-todo-list)
- [Part 6 - Users todo list](https://github.com/wdi-sg/users-todo-list)

## Introduction

> ***Note:*** _This can be a pair programming activity or done independently._

Now that we've written a few tests in our Express application, let's practice writing tests for a more complex application, our TODO list, an app that uses Mongo.

## Exercise

#### Requirements

- Setup the app to run mocha, chai and supertest
- Implement these tests:


```
GET /todos
  ✓ should return a 200 response
  ✓ should return an array
  ✓ should return all the records in the database

GET /todos/:id
  ✓ should return a 200 response
  ✓ should return an object containing the fields 'name', 'description' and 'completed'

POST /todos
  ✓ should return a 200 response
  ✓ should return a 422 response if the field name is wrong
  ✓ should return an error message if the name field is wrong
  ✓ should add a new todo to the database

PUT /todos/:id
  ✓ should return a 200 response
  ✓ should update a todo document

DELETE /todos/:id
  ✓ should remove a todo document
```

* If you include the model todo in your spec file, you can execute requests to MongoDB directly from the test file, allowing you to watch the database directly before or after an action made by a test

**Bonus:**
- Add more validations in the models and add the tests for them, too
- Add fields with different datatypes and write tests for them

#### Starter code

No starter code... use the output of the previous Express Todo Lab.

#### Deliverable


You should expect something like this in the terminal:

![CLI Chai output](http://s23.postimg.org/vt62cg1l7/Screen_Shot_2015_08_12_at_17_13_50.png)


## Additional Resources

- [Chai](http://chaijs.com/)
- [Mocha](https://mochajs.org/)
- [Mongoose Validations](http://mongoosejs.com/docs/validation.html)
