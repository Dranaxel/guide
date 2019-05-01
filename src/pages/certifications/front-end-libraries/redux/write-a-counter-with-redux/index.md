---
title: Write a Counter with Redux
---
## Write a Counter with Redux

In this challenge you have to complete every parts of the counter

Step 1

Modify the constant to accord them with their names :

const INCREMENT = 'INCREMENT'; // define a constant for increment action types
const DECREMENT = 'DECREMENT'; // define a constant for decrement action types

Step 2

Develop the reducer which will handle the actions :

const counterReducer = (state=0, action) =>{
    switch (action.type){
        case (INCREMENT):
            return state +1
        case (DECREMENT):
            return state-1
        default:
            return state
    }
};

Step 3

Create your two actions which will return the type of action accordingly to their name :

const incAction = () =>{
    return {
        type: INCREMENT
    }
};

const decAction = () =>{
    return {
        type: DECREMENT
    }
};

Step 4

Finally 

create the store with the reducer as argument

const store = Redux.createStore(counterReducer);

<!-- The article goes here, in GitHub-flavored Markdown. Feel free to add YouTube videos, images, and CodePen/JSBin embeds  -->
