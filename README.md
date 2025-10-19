# JSLearn Theorey

~> What is EcmaScript ?
:-
EcmaScript is a Standard which defines the syntax,rules and other things for a scripting language. Latest version being used is ES2025

~>What is JavaScript?
:-
Javascript is a scripting language that is based on the standards of ecmascript javascript is the most common scripting language that extends the EcmaScript with functionality such as DOM.


~> How to execute Java Script ?
:-
 1.Javascript can be executed right inside one's browser. You can open the javascript console and start writing javascript there
2.Another way to execute javascript is a runtime like Node.js which can be installed and used to run javascript code.
3.Yet another way to execute javascript is by inserting "it inside <script> tag of an HTML document.
    
~> first program
  // we use console.log() function for printing output in console
  console.log("Hello World");

~> variabls in javascript ?
:- javascript variabls are containers that store data like any other variables
  Var vs Let in javascript
  1 - var is globally scoped while let and const are block scoped
  2 - var can be redeclared and updated withing its scope
  3 - let cannot be redeclared but can be updated
  4 - const can nether be updated not be redeclared
  5 - var variables are initialized with undefined whereas let and const are not initialized 
  6 - const needs to be initialized at decalaration unlike let and var

~> primitive data types and objects
:- primitive data types are those data types are inbuilt or basic data types  
   that are predefined ie their data types and working is predefined
   #there are 7 types of primitive data types in javascript
    1-NULL
    2-Number
    3-String
    4-Symbol
    5-Undefined
    6-Boolean
    7-Bigint

    *Note - we can use typeof keyword to get the type of the variable and this is inbult with node js 

~> Objects in js
:- objects is a userdefined data type that can contain multiple primitive data
    eg:- Creating a object
          const obj={
            name:"Shaurya",
            scholarNo:25204031102
          };

~> Experssion and conditionals 
:- A fragment of code that produces a output is called expression
    operators are logical,assignment,arithmetic,comparision

  
~>conditional statements
:- if , if-else,ladder-if


~> Loops and Functions
:- loops- suppose we are taking multiple inputs from the user then will we take different 
   variables and then write multiple inputs or any such senerio like it so loops help
   us to iterate the same logic multiple times until a condition is statisfied 
  types:-
          1. for loop
              for (let i = 0; i < 5; i++) {
                    console.log("Iteration number: " + i);
              }

          2. for-in loop
              const myObject = { a: 1, b: 2, c: 3 };
              for (const key in myObject) {
                  console.log(`Key: ${key}, Value: ${myObject[key]}`);
              }
          3. for-of loop
              const myArray = [10, 20, 30];
                for (const value of myArray) {
                    console.log(`Value: ${value}`);
                }
                            OR
              const myString = "hello";
                for (const char of myString) {
                    console.log(`Character: ${char}`);
                }
          4. while loop
              var i=0
                while(i<=10)
                {
                  console.log(i++);
                }
          5. do-while loop
              var i=1;
              do{
                printf("I can execute once what ever happens");
              }
              while(i!=1);

   function- funciton is a block of code that promotes code resuablity and helps us to remove redundency 
   from the code , we can keep our code nice and clean where each functionality can be written into a function and 
   this can even help in debugging and further updation in code
      
      -How to make a function in javascript
      //function decalaration and defination
       function helloWorld()
       {
         console.log("Hello World");
       }
       //function calling
       helloWorld();

       or 
       const helloWorld=()=>{
        console.log("Hello World");
       }
       helloWorld();


~>What are Strings?
     
  Strings are basically collection of characters 
  you can declare them using either single quotes or double quotes

  template literals helps us to directly insert variables into strings directly
   
  `I am a string that uses a ${variable} to print it`

  String Functions
  string.length
  string.toUpperCase()
  string.toLowerCase()
  string.slice(start,end) start to end-1
  string.slice(start) start to end of string 
  string.replace() returns new string
  string.concat(string,string) return new string
  string.trim() return new string
  string.includes() return boolean value
  string.indexOf() return index of the first occurance or -1

  Note each function that is updating string returns new string because the strings are immutable 
  in javascript 
  We can access the the characters by the following syntax
  str[index]

~>Array in Javascript
:-Array in javascript are collection of multiple elements that is stored in memmory
  Arrays are Variables which can hold more than one value

    Const fruits = ["banana", "apple", "grapes"]

    const a₁ = [7,"Harry","jatt"]   array can have different types

    Accusing Values
    let numbers = [1, 2, 7, 9]
    numbers [0]->1
    numbers [1]->2

    Finding the length
    let numbers = [1, 7, 9, 21]
    numbers[0]=1
    numbers.length=4

    Changing the Values 
    let numbers=[7, 2, 40, 9]
    numbers[2] = 8

    →"numbers" now becomes [7,2,8,9] Arrays are mutable Arrays can be changed
    typeOf numbers returns prints object

    array functions 
    1. toString() 
      Converts an array to a string of comma separated values
      let n = [1, 7, 9]
      n.toString()->"1,7,9"
    
    2. joins() → joins all the array elements
      using a separator
      let n = [7,9,13]
      n. join ("-") →7-9-13
    
    3. pop() → removes last element from the array
     n = [1,2,4]
     n.pop() 
     updates the original array returns the poped val

    4. push() 
    Adds a new element at the end of the array
    let a = [7,11,2,8]
    a.push(9) modifies the oniginal array
    I reterns the new array length

    5. shift()
    removes an element from the front of the array
    let a = [1,2,4]
    a.shift()
    console.log(a) //prints 2,4

    6. unshift()
    removes an element from the front of the array
    let a =[1,2,3];
    a.unshift(5) /prints 5 1 2 3

    7. delete 
        Array elements can be deleted using the delete operator
        let d = [ 7,8 2 9, 0 ]delete is an operator

    8. Concat()
    used to join arrays to the given array
    let a1 = [1,2,3] 
    let a2 = [ 4,5,6]
    let a3 = [ 9,8, 7]
    a3.Concat(a1, a2)
    return 1,2,3,4,5,6,9,7,8 
    Returns a new array
    Does not change existing arrays

    9. sort()
     sort elements of the array
    
    10. splice()
      helps us to remove and add elemets to an array at the same time
      let array=[1,2,3,4]
      array.splice(location from which elemets are removed,no of elemets,elements to add)
    
    11. slice()
        helps us return a subarray from an existing array
        let arr=[1,2,3,4]
        arr.slice(1) -> Returns [2,3,4]
        arr.slice(1,3) -> Returns [2,3]

    12. reverse()
        helps us to reverse an array

    *Looping through arrays
     1.forEach:traverse each element of an array
        array.forEach((value,index,array)=>{

        })

      2.map:creates a new array by performing function on each element of the array
        array.map((value,index,array)=>{
          return value+1;
        })

      3.filter:helps us to filter elements and removes the elements that do not satisfy the condition
        array.filter((value,index,array)=>{
            return true||false ;
        })
      
      4.reduce:reduces an array to single element;
        array.reduce((accumulator,currentVal)=>{
          return a+b;
        })
      
      5.from:creates an array from another object
        let str="Shaurya"
        console.log(Array.from(str))





~>DOM
:- Dom stands for document object model that makes javascript a powerfull tool 
we will get to know about this further

javascript was initially created to makes the webpages alive ,js can be written in a web page's html to make it interactive 
the browser has an embedded engine calles the javascript engine or the javascript runtime

Dev tools
:-Every browser has some developer tools which makes a developer's life a lot easier
its shortcut on chrome is F12

Do you know that javascript can be written in javascript console

the <script> </script> tag can be used to insert internal or external script in the code

the benefit of a seprate js file is that the browser will download it and store it in its chache

# JSLearn


