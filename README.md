# Práctica Vue.js Fundamentals

Estudiante: Laura Manzini - *alu0101531700@ull.edu.es*

## Introduction

This repository is a template for you to follow the course [Vue.js Fundamentals](https://vueschool.io/courses/vuejs-fundamentals).

This Vue.js course [Vue School](https://vueschool.io/courses/vuejs-fundamentals) will teach you and get you up and running with the basics concepts of Vue.js. 

You can find this free course by **Vue School** at [vueschool.io](https://vueschool.io/courses/vuejs-fundamentals). 
The course is suitable for developers who do not yet know about Vue.js or are just getting started with Vue.

See also [Annotated Reading of the Essentials Section of the Vue.js Guide](https://crguezl.github.io/learning-vue-geting-started-guide)

## TODOS for the Shopping list app

Follow these steps:

- [x] Write initial HTML with a shopping-list div
- [x] Load and Instanciate Vue add data and Vue template syntax to interpolate
- [x] Add an input an synchronize it with the interpolated text to see it
- [x] Explore the app in the console
- [x] Discuss the syntax of JS inside moustaches
- [x] Learn to read the errors in the console
- [x] Add items to data and show them using v-for
- [x] Add input a variable to store the newItem
- [x] Connect the input with the newItem and check the binding
- [x] Use Vue Devtools. Configure it to work with file://
- [x] Add v-on: Start by simulating in the console what we are going to do
- [x] Add button to add the new item when clicked
- [x] Add v-on:keyup.enter to the input element
- [x] Shorthands for v-on 
- [x] Use a method `saveItem` to factorice
- [x] Reset the input when finished the insertion
- [x] Check the method using the debugger
- [x] v-if and v-else: add a conditional message when the list is empty


### Next Steps: Add State to your App

- [x] Add a `state` variable to the app `data` to represent the states of the app. 

  There will be two states: **default** and **edition**. 
  The views on each state will be different

  State **edition** corresponds to when the user is adding/editing a new item: there will be an **input** form to input the item, buttons to **cancel** the edition, to **save the item**, etc.

  State **default** corresponds to when the user is the initial state. There will be a button to **add** a new item 


- [x] Move the `input` and `button` *Save Item* elements to a `div` with class `add-item-form` so that these styles apply

  ```css
  .add-item-form, .header {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .add-item-form input {
      width: 70%;
      border-radius: 3px;
      box-shadow: 0 2px 4px 0 rgba(0,0,0,0.10);
      border: 1px solid #F1F5F8;
      color: #606F7B;
      padding: .5rem .75rem;
      box-sizing: border-box;
      font-size: 1rem;
      letter-spacing: .5px;
      margin: .5rem 0;
  }
  ```
- [x] Show the `div` with class `add-item-form` only if the state is `edition`
- [x] To the div with class `header` add a button `Add Item` that will make the app transit from the `default` state to the `edition` state 
- [x] Show the  `add button` only if the state is `default` 
- [x] To the div with class `header` add a button `Cancel Adding Item` with the class `btn-cancel` that will make the app transit from the `edition` state to the `default` state 
- [x] Show the  `Cancel Adding Item` button only if the state is `edition`
- [x] Add the `changeState` method that reflect the transitions between both states 


## v-bind steps

- [x] Using the dev tools, check that when we click the `save item` with the `input` empty we are adding new empty strings to the `items` list
- [x] Disable the button `save item` when the `input` is empty by binding the `disabled` attribute of the button

  The `disabled` attribute is a boolean attribute. A disabled button is unusable and un-clickable.
  
  The disabled attribute can be set to keep a user from clicking on the button until some other condition has been met (like selecting a checkbox, etc.)

## Dynamic classes with v-bind

- [x] Change the list of items from a list of Strings to a list of Objects with `label` and `purchased` attributes. Update the `saveItem` method and the template accordingly
- [x] Make use of the class `.strikeout` in the css file:

  ```css
  .strikeout {
    text-decoration: line-through;
    color: #B8C2CC;
  } 

  .strikeout:hover {
      color: #8795A1;
  }
  ```

  to style the purchased items. See the [Vue.js Guide section on Class and Style Bindings](https://vuejs.org/v2/guide/class-and-style.html)
  - [x]  Use first the *object syntax* `v-bind:class="{myclass: expression}"` and 
  - [x]  later the *array syntax* `v-bind:class=[exp1, exp2]`


## Topics

- Introduction to two-way data binding
- Template syntax and expressions
- Vue directives, loops and conditional rendering
- Vue Devtools
- Handling user Inputs
- Handling Events
- Vue.js Methods and Computed Properties
- Attribute Bindings and dynamic classes
- Components


## Further details

For more details on the introduction to Vue please follow this [repository](https://github.com/ULL-ESIT-DMSI-1920/vue-intro-laura-manzini-alu0101531700.git).







