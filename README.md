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
    Unlike most languages where array is a reference to the multiple variable, in JavaScript array is a single variable that stores multiple elements. To instiate Array we use [] brackets. Basic syntax of object 
        
        var House = []; // Some value in it.

In Javascript array and object are almost same, Array also a object but object is not an array.
Main advantage of Array that Array have some cool methods like ``` array.push() ``` ```arrray.map()``` we also can use ``` array.length ```.
In array data is sorted by index, Array are always orderd but in objects data gets stored by key value pair and it's unordered.


#### Destructing
    A Simplified way of defining variables & tkaing them outside of an object or an array.
        
        * Array
        let [first, second] = [true, false]
        const [first, second] = [true, false]
        var [first, second] = [true, false]

    
    
    
Skipping
            
            var [a, , b] = [1, 2, 3] // => [1, 3]

Swapping
        
    var a = 1, b = 2; then [b, a] = [a, b]
.
    
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

var is Javascript have the function scope, JS use  [hositing](#Hoisting) that's why use can use var before it's declare. you can access every where in your function.
        
##### Hoisting
While variables declared with var keyword are "hoisted" to the top of the block which means they are accessible in their enclosing scope even before they are declared:
        
        function run() {
            console.log(foo); // undefined
            var foo = "Foo";
            console.log(foo); // Foo
        }
        run();

##### Global Variables

Global veriables get's declare without any prefix like ```ACTUAL``` this is the global variable. or we declare  ```window.actual``` this is the variable in entire codebase.

###### Spread Operator
The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

    const numbers = [1, 2, 3];
    console.log(sum(...numbers));

or
    
    var [a, ...b] = [1, 2, 3] // => 1, [2, 3]

### Scopes

Scope is the accessibility of variables, functions, and objects in some particular part of your code during runtime. In other words, scope determines the visibility of variables and other resources in areas of your code.

JavaScript has three types of scopes.
 * Global scopes
 * Outer scopes
 * Inner scopes

 ##### Globla Scope
 When you start writing JavaScript in a document, you are already in the Global scope. There is only one Global scope throughout a JavaScript document. A variable is in the Global scope if it's defined outside of a function.

        // the scope is by default global
        var name = 'Hassan';

##### Outer Scope
    JavaScript outer scope is like access value from it's parent functions. variable define in the parent  of calle function.

##### Inner/local Scope
Variables defined inside a function are in the local scope. And they have a different scope for every call of that function. This means that variables having the same name can be used in different functions. This is because those variables are bound to their respective functions, each having different scopes, and are not accessible in other functions. 

### Functions
A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:

* The name of the function.
* A list of parameters to the function, enclosed in parentheses and separated by commas.
* The JavaScript statements that define the function, enclosed in curly brackets, {...}.

##### Closures
Closures are one of the most powerful features of JavaScript. JavaScript allows for the nesting of functions and grants the inner function full access to all the variables and functions defined inside the outer function (and all other variables and functions that the outer function has access to).

    var pet = function(name) {   // The outer function defines a variable called "name"
    var getName = function() {
    return name;             // The inner function has access to the "name" variable of the outer 
                             //function
    }
      return getName;            // Return the inner function, thereby exposing it to outer scopes
    }
    myPet = pet('Tomy');
   
    myPet();     // Returns "Tomy"

##### High Order Functions.
High order functions enable us to do these functional programming techniques is JS.
High order functions and callbacks are the core concepts of functional programming , it's very powerfull too.
High order functions takes a function as input, we can also return a function as output.

        document.on('click','body', function(){
            return () => { console.log('Learning JS') };        
            })

##### Anonymous function
    Anonymouns have without have any name. they are also called arrow functions.
    e.g  () => return true.
## Array Methods
Arrays provide a lot of methods. To make things easier, in this chapter they are split into groups.

* foreach()
    
    The forEach() method executes a provided function once for each array element.
        
        const array1 = ['a', 'b', 'c'];
        array1.forEach(element => console.log(element));

        // expected output: "a"
        // expected output: "b"
        // expected output: "c"

    foreach method doesn't return any thing.

* map()

The map() method creates a new array populated with the results of calling a provided function on every element in the calling array.

    const array1 = [1, 4, 9, 16];

    // pass a function to map
    const map1 = array1.map(x => x * 2);

    console.log(map1);
    // expected output: Array [2, 8, 18, 32]

map return an array of updated values.


* arr.push()
    
    The push() method adds one or more elements to the end of an array and returns the new length of the array.
    
        const animals = ['pigs', 'goats', 'sheep'];
        const count = animals.push('cows');
* arr.pop()

The pop() method removes the last element from an array and returns that element. This method changes the length of the array.
            
        const plants = ['broccoli', 'cauliflower', 'cabbage', 'kale', 'tomato'];
        console.log(plants.pop());
        // expected output: "tomato"
* arr.shift()

    Extracts an item from the beginning,
    
        const array1 = [1, 2, 3];
        const firstElement = array1.shift();
        console.log(array1);
        // expected output: Array [2, 3]

* arr.unshift(...items)

    Adds items to the beginning.
    The unshift() method adds one or more elements to the beginning of an array and returns the new length of the array.

        const array1 = [1, 2, 3];
        console.log(array1.unshift(4, 5)); // expected output: 5
        console.log(array1); // expected output: Array [4, 5, 1, 2, 3]
    
* splice()

    The splice() method changes the contents of an array by removing or replacing existing elements and/or adding new elements in place.

        const months = ['Jan', 'March', 'April', 'June'];
        months.splice(1, 0, 'Feb'); // inserts at index 1
        console.log(months); // expected output: Array ["Jan", "Feb", "March", "April", "June"]

* concat()

    The concat() method is used to merge two or more arrays. This method does not change the existing arrays, but instead returns a new array.
        
        const array1 = ['a', 'b', 'c'];
        const array2 = ['d', 'e', 'f'];
        const array3 = array1.concat(array2);

        console.log(array3); // expected output: Array ["a", "b", "c", "d", "e", "f"]

* filter()

    The filter() method creates a new array with all elements that pass the test implemented by the provided function.

        const words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];
        const result = words.filter(word => word.length > 6);
        console.log(result);
        // expected output: Array ["exuberant", "destruction", "present"]






    


















