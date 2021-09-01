# Putting it all together
In this document you are going through subjects that will help you build a searchable data table using react. the example that we will provide will be related to a product table.  

## Break a mock into a component hierarchy:

To make a hierarchy of components, you need to identify them (the components) first. This is a topic for debate, because you might look at things differently than other people. However, there are things that need to be in your mind.  

- The _**single responsibility principle**_, which means that a function or a component need to do a single thing, and if it get bigger, it might need to be disassembled to smaller functions or components.  

- The relations between components. A low/medium-fidelity-wireframe that shows all the components of you App with marks on how each components relate to the other will help allot.  
![lfw](imgs/lfw.png)  

According the the previous LFW, you can see 5 components, each is marked in a box. The outer boxes represent father components and the inner boxes the children.

Form that you can assign this hierarchy:  
1. **FilterableProductTable (orange)**: contains the entirety of the example
1. **SearchBar (blue)**: receives all user input
1. **ProductTable (green)**: displays and filters the data collection based on user input
1. **ProductCategoryRow (turquoise)**: displays a heading for each category
1. **ProductRow (red)**: displays a row for each product.  


## Build a ‘static’ version of your application

After finishing from defining the components and their relationships to each other, you can start building the app. the app should be static, which requires more typing and less thinking.   

In this stage, you would be building the components and passing `props` from one to another. You are not going to use `states`, because you are building a static app.  

You can decide how to build your app, top-down or bottom-top. However, usually small apps are better worked on top-dow, while larger apps are better suited with bottom-top.  

Render you components, and at the end you would have an library of reusable components, and ready to be adjusted to be interactive., by adding `states`. 

## Identify The Minimal (but complete) Representation Of UI State

The first step into making your app dynamic is to identify your states.

You can ask three questions to decide what is state anf what is not:  

- Is it passed in from a parent via props? If so, it probably isn’t state.  
- Does it remain unchanged over time? If so, it probably isn’t state.
- Can you compute it based on any other state or props in your component? If so, it isn’t state  

If we looked at our pieces of data from our previous example, we wil have 4 pieces:

1. The original list of products
1. The search text the user has entered
1. The value of the checkbox
1. The filtered list of products  

You can draw a conclusion that we have 2 states in app:

- The value of the checkbox.
- And the search text the user will enter.

## Identify Where Your State Should Live

Now you must conclude where your state should live, and what component should hold it and receive its updates.  

To help you decide think about the following: 

* Identify every component that renders something based on that state.
* Find a common owner component (a single component above all the components that need the state in the hierarchy).
* Either the common owner or another component higher up in the hierarchy should own the state.
* If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.  

For our example, we can conclude the following:  

* **ProductTable** needs to filter the product list based on search state and **SearchBar** needs to display the search text and checked state.
* The common owner component is **FilterableProductTable**.
* It conceptually makes sense for the filter text and checked value to live in **FilterableProductTable**.  

## Add Inverse Data Flow  

If you did all the previous step, then your app is nearly finished. All is needed now is to add some functions and pass them from their component to related components, to updated the `stets` and make your app dynamic.  

In out example, we add to functions, that sets the states using `setState()` function of the checkbox and user inputs. and then we have passed them to the components that are responsible of rendering the data.  

Where the user well enter the data, we made `onChange` functions, so the state will be changed at the moment the user enters it.  


