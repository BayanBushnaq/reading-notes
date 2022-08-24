# React and Forms

## React Docs - Forms
### What is a ‘Controlled Component’?

#### Controlled Components are those in which form's data is handled by the component's state.
#### It takes its current value through props and makes changes through callbacks like onClick

### Should we wait to store the users responses from the form into state when they submit the form 
### OR should we update the state with their responses as soon as they enter them? Why.

#### because we uswed Controlled Component we have to wait to store the users responses from the form into state. 


### How do we target what the user is entering if we have an event handler on an input field?

####  controlled component prevents the user from changing the input unless you desire so. If you’ve specified a value but the input is still editable,
#### you may have accidentally set value to undefined or null.

# The Conditional (Ternary) Operator Explained

## Why would we use a ternary operator?

####  for decision making in place of longer if and else conditional statements. 


## Rewrite the following statement using a ternary statement:

#### (x===y) ? console.log(true) : console.log(false) ;
