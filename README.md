# Project: Week 1: To-do list application
## Introduction
As a team, you should create and style the front-end of a to-do list web application using React and Material UI components. A typical user wants to be able to use a to-do list to organize tasks. Keeping user stories in mind when designing applications helps determine important features. We encourage you to take a unique approach to this lab as there is no one right answer. 
- [Material Design](https://material.io/design/introduction) is a design system that can guide you on what UI decisions to make if you would like to explore best practices, but functionality is the key focus of the lab.
- No back-end is required for this lab, all data (tasks) should live in the front-end.


## Requirements
Feature requirements (Week1 task is complete when you):
+ Design your personalize about me page
+ **Take in and display** to do list items

Implementation requirements:
+ Use [**Material UI components**](https://material-ui.com/) at least once throughout the app
+ Implement at least one **functional component**

## Instructions/Hints:

### About Page
Note: The styling for this page `About.css` is provided for you. However, feel free to play around with the styling to gain better understanding of how they work.
1. Natigate to src/pages/About.js. Replace the `p` tag with your content. Your content should include:
    - A picture
    - Details about you like Interests, fun fact so on...
    To achive this, consider using div tags to split the page in half like so
    ```
     <div>
        <div class="split left">
          <div className="centered">
            <img 
              className="profile_image"
              // Image goes here
              alt="Profile Pic"
              ></img>
          </div>
        </div>
        <div className="split right">
          <div className="centered">
            <div className="name_title">Your Name</div>
            <div className="brief_description">
              // Details about you goes here
            </div>
          </div>
        </div>
      </div>

    ```
2. Upload your profile picture into the assets folder. i.e /src/assets/<profile_pic_name.jpg>
3. Import About.css file and profile picture in your About.js file like so 
    ```
    import "./About.css";
    import <profile_pic_name> from "../assets/profile_pic_name.jpg";
    ```
### TO-DO List APP
1. Create two components `AddTodo.js` and `todo.js`  in the src/component/ directory
    + `AddTodo.js` Create a class with an HTML form and textFiled which takes in list of todo items.
    + 
    + `todo.js` Create a function that helps to hold and return the todo list
2. Import both files in your Home.js file.
3. Create a function that add items to the list and renders the html elements need to display the list on the page.
   Sample add function 
   ```
    addTodo = (todo) => {
        todo.id = Math.random();
        let todos = [...this.state.todos, todo];
        this.setState({
            todos: todos,
        });
    };
   ```


## Testing
When testing web components, developers often use ids to uniquely define elements on a page. The React Testing Library provides a query which can identify items with the attribute data-testid to do just that (reference [here](https://testing-library.com/docs/queries/bytestid/)). We have implemented simple tests in `App.test.js` that will look for ids in your code. Do not push changes to the tests in this file. To get familiar with the idea of testing ids, implement the attributes below:
+ `data-testid="new-item-input"` on the Input component which takes user input for new items.
+ `data-testid="new-item-button"` on the Button component which submits new items to the to do list.


Note: Material UI components (and other libraries) render as HTML components under the hood, so using Material UI's TextField would still render in the DOM as an Input element and pass the tests for this lab.

## Pre-session Material
Here is a [**link**](https://ibm.ent.box.com/folder/163593416418) to the pre-session material that was provided to you earlier.

