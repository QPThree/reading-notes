# Passing Functions as Props

## In this Article

[React Docs - Lists & Keys](#topic1)

[The Spread Operator](#topic2)

[How to Pass Functions Between Components](#topic3)

---

<a name="topic1"></a>

## React Docs - Lists & Keys

1. What does .map() return?
The *.map()* function returns an array by design. No extra coding required from the developer.
2. If I want to loop through an array and display each value in JSX, how do I do that in React?
You can simply write the JSX in the return of your function. The javascript variables can be accessed by putting them inside of curly  braces.
3. Each list item needs a unique ____.
Key associated with it.
4. What is the purpose of a key?
Keys allow React to detect which item shave been changed or added. React will "re-render" the page and components based on the changes made. 
<a name="topic2"></a>

## The Spread Operator

1. What is the spread operator?
A quick syntax method that can perform various actions on or with arrays. 
2. List 4 things that the spread operator can do.

* Add items to an array

* Combine arrays or objects

* Spreads an array into separate objects as a functions argument

* Useful when concatenating arrays

3. Give an example of using the spread operator to combine two arrays.

> const arrOne = ['a', 'b', 'c'];
> const arrTwo = [1, 2, 3];
> const arrThree = [...arrOne, ...arrtwo];
> console.log(...arrThree) // abc123

4. Give an example of using the spread operator to add a new item to an array.

> const arrTwo = [1, 2, 3];
> const moreNumbers = [-1, -2, ...arrTwo]
> console.log(moreNumbers) // [-1, -2, 1, 2, 3]

5. Give an example of using the spread operator to combine two objects into one.

> const objectOne = {firstName: "Quentin"}
> const objectTwo = {lastName: "Young"}
> const person = {...objectOne, ...objectTwo}
> console.log(person) // {firstName: "Quentin", lastName: "Young" }

<a name="topic3"></a>

## How to Pass Functions Between Components

1. In the video, what is the first step that the developer does to pass functions between components?

> answer: They create a function on the level the state exists that sets the state.

2. In your own words, what does the increment function do?

> The function increase the count value of an object in the app.js state.  The object to update is determined by the name that is passed to the function. If it matches an objects 'name', then that objects count is incremented.

3. How can you pass a method from a parent component into a child component?

Just like you would any other prop.  Once the method is passed to a child, the child component can use it like any of the other methods. 
4. How does the child component invoke a method that was passed to it from a parent component?

The child component, for example, could have a function called 'increment' that calls the prop passed into it. You can simply call the prop, 'this.prop.increment()' inside of the child's own 'increment' function. The prop would be the function passed into the child, from the parent. And that part is key.  The child cannot see or access that function unless it is passed into it. 

~ QP3

[Home](../README.md)

