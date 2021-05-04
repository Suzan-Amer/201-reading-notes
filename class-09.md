# Read: 09 - Forms and Events

# Forms

## Why Forms?
### The best known form on the web is probably the search box that sits right in the middle of Google's homepage.


## Form Controls
 * ADDING TEXT: 
    * ***Text input*** (single-line)Used for a single line of text suchas email addresses and names.
    * ***Password input*** Like a single line text box but it masks the characters entered.
    * ***Text area*** (multi-line) For longer areas of text, such as messages and comments.
* Making Choices: 
   * **Radio buttons**  For use when a user must select one of a number of options.
   * ***Checkboxes*** When a user can select and unselect one or more options.
   * ***Drop-down boxes*** When a user must pick one of a number of options from a list 
* Submitting Forms:
  * ***Submit buttons*** To submit data from your form to another web page.   
  * ***Image buttons*** Similar to submit buttons but they allow you to use an image.
* Uploading Files:  
   * ***File upload*** Allows users to upload files e.g. images) to a website.


![form](https://cdn.wallstreetmojo.com/wp-content/uploads/2019/08/Form-Controls-in-Excel-Example-1.1.png)

## How Forms Work?
#### 1- A user fills in a form and then presses a button to submit the information to the server.
#### 2- The name of each form control is sent to the server along with the value the user enters or selects.
#### 3- The server processes the information using a programming language such as PHP, C#, VB. /net, or Java. It may also store the information in a database. 
#### 4- The server creates a new page to send back to the browser based on the information received.

## Form Structure
* <**form**>
    - Form controls live inside a <*form*> element. This element should always carry the action attribute and will usually have a method and id attribute too.

* **action**
  * Every <*form*> element requires an action attribute. Its value is the URL for the page on the server that will receive the information in the form when it is submitted. 

* **method**
   * Forms can be sent using one of two methods: get or post.    

![f](https://1.bp.blogspot.com/-jgPYBhN-ioM/XRchsiRV66I/AAAAAAAAFsY/KO9TxrR2lV8ZhfPeGkKOJxVb5XJBZ3j7ACLcBGAs/s640/1.JPG)   

## text input code 

!][im](https://cdn.educba.com/academy/wp-content/uploads/2019/06/html1.png)

## Password Input code 
![pass](https://cdn.educba.com/academy/wp-content/uploads/2019/06/html7.png)

## Radio Button
![radio](https://juristr.com/blog/assets/imgs/radiobuttonsbinding.png)



# list style type
![ls](https://cloud.netlifyusercontent.com/assets/344dbf88-fdf9-42bb-adb4-46f01eedd629/7db7b396-48da-4e19-9df5-ed21d9de5d39/list-markers.jpg)

## types for list 
 * list-style-type
 * list-style-image
 * list-style-position
 * list-style
 

## Table 

![table](https://cf2.ppt-online.org/files2/slide/x/x03e9GTk5pRrMdEywnDSZbjBHJ2zoYaFmfuKsh/slide-1.jpg)

#

## FOCUS & BLUR EVENTS
### The HTML elements you can interact with, such as links and form elements, can gain focus. These events fire when they gain or lose focus.
### The focus and b 1 ur events are most commonly used on forms. They can be particularly helpful when:
* You want to show tips or feedback to users as they interact with an individual element within a form (the tips are usually shown in other elements and not the one they are interacting with)
* You need to trigger form validation as a user moves from one control to the next (rather than waiting for them to submit the entire form first)


## HOW EVENTS TRIGGER JAVASCRIPT CODE
### When the user interacts with the HTML on a web page, there are three steps involved in getting it to trigger some JavaScript code. Together these steps are known as event handling.
* Select t he element node(s) you want the script to respond to.
* Indicate which event on the selected node(s) will trigger the response.
* State the code you want to run when the event occurs.

## MOUSE EVENTS
## The mouse events are fired when the mouse is moved and also when its buttons are clicked.
### All of the elements on a page support the mouse events, and all of these bubble. Note that actions are different on touchscreen devices.
### Preventing a default behavior can have unexpected results. E.g., a click event only fires when both the mousedown and mouseup event have fired.

![mus](https://www.javascripttutorial.net/wp-content/uploads/2020/02/javascript-mouse-event-screenX-screenY.png)
## USING MUTATION EVENTS

### In this example, two event listeners each trigger their own function. The first is on the last but one line, and it listens for when the user clicks the link to add a new list item. It then uses DOM manipulation events to add a new element (changing the DOM structure and triggering mutation events).
### The second event listener waits for the DOM tree
### within the <**ul**> element to change. When the DOMNodelnserted event fires, it calls a function called updateCount ().This function counts how many items there are in the list, and then updates the list count at the top of the page accordingly.
 
 ## summaary 
* Events are the browser's way of indicating when something has happened (such as when a page has finished loading or a button has been clicked).
* Binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon.
* When an event occurs on an element, it can trigger a JavaScript function. 
* When this function then changes the web page in some way, it feels interactive because it has responded to the user.
* You can use event delegation to monitor for events that happen on all of the children of an element.
* The most commonly used events are W3C DOM events, although there are others in the HTMLS specification as well as browser-specific events.



# Some questions to refresh your mind :
##  **q1** How Forms Work?
## **q2** Mention the list types?
## **q3**  HOW EVENTS TRIGGER JAVASCRIPT CODE?