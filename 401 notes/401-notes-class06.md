# Class-06 Notes:

1.  Explain what a “Singleton” is in Computer Science terms

    - [SOURCE](<https://en.wikipedia.org/wiki/Singleton_pattern#Singleton_classes_do_not_allow_for_test-driven_development_(TDD).>)
    - Singleton is a type of software design pattern that restricts instantiation of a class to a **single** instance.
    - also involves hiding of a class's constructor so that it connat be instantiated outside the class.

2.  Explain how the Singleton pattern can be used with Node modules, specifically with classes

    - [SOURCE](https://medium.com/swlh/node-js-and-singleton-pattern-7b08d11c726a)
    - for every class we want to apply the singleton patter to, we create a second, private class that alone can be used to create an instance.

    ```js
    class PrivateSingleton {
      constructor() {
        this.message = "I am an instance";
      }
    }
    class Singleton {
      constructor() {
        throw new Error("Use Singleton.getInstance()");
      }
      static getInstance() {
        if (!Singleton.instance) {
          Singleton.instance = new PrivateSingleton();
        }
        return Singleton.instance;
      }
    }
    module.exports = Singleton;
    ```

## Vocabulary

- `Dynamic Module Loading`: when a computer progam loads a library it needs at runtime. we use this method to import things like Express, Jest, mongoose, etc
- `Singleton Patter`: a type of software design pattern that restricts instantiation of a class to a **single** instance.
- `CRUD`: stands for CREATE-post/put, READ-get, UPDATE-put/post/patch, DELETE-delete.
- `Mock Testing`: a way of unit testing code that allows you to make assertions about how the code being test is interacting with other modules. Dependencies are replaced with objects that simulate the behaviouur of the real ones. [SOURCE](https://devopedia.org/mock-testing#:~:text=Mock%20testing%20is%20an%20approach,behaviour%20of%20the%20real%20ones.)

1. Despite how powerful encryptions are, inputs can still be crack through brute force methods. I also have a better understanding of both Authentication paradigms. and I also see that that are multiple ways to hash a password.
2. I'm hoping to learn more about more ways of hashing user info. and more about Bearer Authentication.
