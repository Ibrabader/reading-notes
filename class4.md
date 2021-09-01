# React and Forms
## Forms  

### Controlled Components
_**controlled components**_ : is technique when dealing with React, that allows JavaScript to have access to the data that the user entered into the form. Then analyze the data and do modification.  

- In typical `HTML`, forms elements maintain their states, and only update based on user inputs. However, in **React**, multiple state properties are processed in a component and only updates with `setState()`.

- You can combine both `HTML` and `React` methods by the
“`controlled component`”.

- An input form element whose value is controlled by **React** in this way is called a “`controlled component`”.  
  
![both](./imgs/both.png)  
- in this example the value in the form is passed as a state, so React state will always be the source of the value. By making the user input a state, you can use pass that state to other components and use it there.

### The textarea Tag

- `<textarea>` defers in `React`, by that its value is passed through a `value attribute`. This allows you to store it as a React state and make **React** the source of it value. And give it an initial value too.  
![text](imgs/textarea.png)   

### The select Tag

- `<select>` is similar to `<textarea>` in **React**, but you can also, make an option selected by using `value attribute` on the root `select` tag. Also, you can just like `<textarea>` make the source of its value  `this.state`.
![select](imgs/select.png)  

### The file input Tag

- `<input>` in **React** is deferent than `HTML`by that, it is discussed together with other uncontrolled components

### Handling Multiple Inputs

- Just like normal `JavaScript`, you can add `name` attributes to multiple inputs, and then identify each input by it attribute. The diffrence that in **React** you can control their values through `this.state` and `setState()` by the **handler function**.

### Controlled Input Null Value

- By using `setTimeout()` function, you can delay the ability to edit an input by predefined time to prevent having `null` or `undefined` values.

![delay](imgs/delay.png)  

### Alternatives to Controlled Components

-  _**uncontrolled components**_, is an alternative technique for implementing input forms. Instead of using _**controlled components**_, and defining function to each input so it can be handled.

## The Conditional (Ternary) Operator Explained

- "_**conditional ternary operator**_" is a shorthand for writing `if` statements in one line.  
instead of this:  

```
if (person.age >= 16) {
  person.driver = 'Yes';
} else {
  person.driver = 'No';
}

```

you can write as this:  

`person.driver = person.age >=16 ? 'Yes' : 'No';`  

### The Conditional (Ternary) Operator  

- Here’s what you need to know:  
    1. The `condition` is what you’re actually testing. The result of your condition should be true or false or at least coerce to either boolean value.
    1. A `?` separates our conditional from our `true` value. Anything between the `?` and the `:` is what is executed if the condition evaluates to `true`.
    1. Finally a `:` colon. If your condition evaluates to `false`, any code after the colon is executed.

### Notes:

- You can nest **(Ternary) Operator** inside of each other to test for multiple conditions.  
![multi-con](imgs/multi.png)  

- You can also, do multiple operations using **(Ternary) Operator**, by separating each line with a **comma**, and you can group your code by using parenthesis.    
![multi-ope](imgs/multi2.png)  

- example: `x===y ? console.log('true') : console.log('false')`  
