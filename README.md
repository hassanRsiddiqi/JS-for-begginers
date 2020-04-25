# JS-for-begginers
This repository is about to those who are new in JS, want to know about JS, Some Basic and advance feature, ES6, Arrays, Objects and much more.

Let's start.

Before starting this I'll prefer you should have some basic knowledge of HTML & CSS. 
If you take an example of house, HTML is like the gray structure of our house, CSS do some decoration stuff, like painting, coloring etc, like this JS make our house use able, Like we can switch on our light, fan. Js give us the control, we can move the things with the JS.

In this repoistory I'll talk about the JavaScript, Basically JavaScript is the scripiting programming language, that allow us to implement the complex feature on our website. these days JS used in almost every web site. there are over [1.6 billion websites](https://www.internetlivestats.com/total-number-of-websites/) in the world and JavaScript is used on 95% on them. 1.52 billion web sites with JavaScript. Javascript is the powerfull language, you can create almost all type of application with this, like Native Mobile apps, desktop applications, iOT devices.

JavaScript is a multi-paradigm language that allows you to freely mix and match object-oriented, procedural, and functional paradigms. 

Immutability is a core tenet of functional programming. It, along with pure functions, makes it easier to reason about and debug your programs.

Functional programming is about the verbs.
Object oriented programming is about the nouns.


In JS we use **var**, **let** & **const** to declare the variables. these three are differnet by scopes we will look into deep leter in this article.

JavaScript defines **seven** built-in types:

Type: A type is an intrinsic, builtin set of characteristics that uniquely identifies the behavior of a particular value and distinguishes it from other values, both to the engine and to the developer.

* null
* undefined
* boolean   
* number
* string
* object
* symbol—added in [ES6!](https://medium.com/@rogercodes1/what-is-es6-ecmascript-6-the-standard-of-javascript-and-its-features-c05a7d2ccc9d)

```
    typeof undefined === "undefined"; // true
    typeof true === "boolean"; // true
    typeof 42 === "number"; // true
    typeof "42" === "string"; // true
    typeof { life: 42 } === "object"; // true
    // added in ES6!
    typeof Symbol() === "symbol"; // true
```
All of these types except object are called
“primitives.” 
* ### Prmitive
    Any thing that is not an object called Prmitive value.
    Prmitive gets its own spot in memory. they have their seperate block in memory.
    it can be string, number, boolean, symbol, null, undefined.

* ### Non Prmitive Value 
    Non primitive value share the same place in memory. if you change the non prmitive value it can change things in un usual ways.

For storing the run time value Javascript use the Object & Array.
* #### Object
        Object are used to represent a “thing” in your code. That could be a person, a car, a building, a book, 
        a character in a game — basically anything that is made up or can be defined by a set of characteristics. 
        In objects, these characteristics are called properties that consist of a key and a value.

        To instiate objects we use {} brackets.
        Basic syntax of object .

        var object = {
            key: 'value'
        }; 
            
* #### Array
        In JavaScript, array is a single variable that is used to store different elements.
        It is often used when we want to store list of elements and access them by a single variable.
        Unlike most languages where array is a reference to the multiple variable, in JavaScript array is a single variable that stores multiple elements.
        To instiate Array we use [] brackets.
        Basic syntax of object 
        var House = []; // Some value in it.

In Javascript array and object are almost same, Array also a object but object is not an array.
Main advantage of Array that Array have some cool methods like ``` array.push() ``` ```arrray.ma()``` we also can use ``` array.length ```.
In array data is sorted by index, Array are always orderd but in objects data gets stored by key value pair and it's unordered.


#### Destructing
        A Simplified way of defining variables & tkaing them outside of an object or an array.
        
        * Array
        let [first, second] = [true, false]
        const [first, second] = [true, false]
        var [first, second] = [true, false]

        When it comes to array the assigment will be based on order, first value will be assign to first and second value will be passed to second one and so on.
        like: first = true, second = false

        * Object
        let { first, second } = { first: true, second: false }
        const { first, second } = { first: true, second: false }
        var { first, second } = { first: true, second: false }

        When we are using objects the order doesn't matters, it works on the object key. like first will be look on the right side obeject and will find the same name key.

### Assignment
        we can reassign already declare values like this.
        [first, second] = [first, second]
    
        In this way we can assign multiple variable in a single line. or else we can write like this.
        first = true;
        second = false;

let's talk about let, const & var.
    
var and let & const are used for variable declaration in javascript but the difference between them is that var is function scoped and let & const are block scoped.
It can be said that a variable declared with var is defined throughout the program as compared to let and const.

Different between let and const is that, we can re assign some value to let, but we can't reassign the value to const becuase cosnt just create the readable refrence in memory, if we just try to change the value of const, it will led us with the error.

both let are const are block scope value. 

Block is JavaScript is between of {} curely braces.

Curly braces {} are used to define the scope of Class, functions, confition etc.

        () braces use to call the function. 
for example. 

        let fun = () => console.log('hello')
if we will just console the fun it will print the syntax of the functions.

        console.log(fun);  // () => console.log('hello')

if we console it with () then it will execute the function and will print the result.

        console.log(fun()); // hello







