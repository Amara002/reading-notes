# Forms
***Traditionally, the term 'form' has referred to a printed document that contains spaces for you to fill in information.***

## Why Forms?
***The best known form on the web is probably the search box that sits right in the middle of Google's homepage.***

## Form Structure
***Form controls live inside a '< form >' element. This element should always carry the action attribute and will usually have a method and id attribute too.***

## Text Input
***The '< input >' element is used to create several different form controls. The value of the type attribute determines what kind of input they will be creating.***

## Text Area
***The '< textarea >' element is used to create a mutli-line text input. Unlike other input elements this is not an empty element. It should therefore have an opening and a closing tag.***

## Radio Button
***type="radio"Radio buttons allow users to pick just one of a number of options.***

## CheckBox
***type="checkbox"Checkboxes allow users to select (and unselect) one or more options in answer to a question.***

## Submit Button
***type="submit"The submit button is used to send a form to the server***

## Image Button
***type="image"If you want to use an image for the submit button, you can give the type attribute a value of image. The src, width, height, and alt attributes work just like they do when used with the '< img >' element***

## Button & hidden Controls
***type="hidden"This example also shows a hidden form control. These form controls are not shown on the page (although you can see them if you use the View Source option in the browser). They allow web page authors to add values to forms that users cannot see. For example, a web page author might use a hidden field to indicate which page the user was on when they submitted a form.***

## Labelling Form Controls
***'< label >':When introducing form controls, the code was kept simple by indicating the purpose of each one in text next to it. However, each form control should have its own '< label >' element as this makes the form accessible to vision-impaired users.***

## Grouping Form Elements
- ***You can group related form controls together inside the '< fieldset >' element. This is particularly helpful for longer forms.***
- ***The <legend> element can come directly after the opening '< fieldset >' tag and contains a caption which helps identify the purpose of that group of form controls.***

##  Email & URL Input
- ***type="email" If you ask a user for an email address, you can use the email input. Browsers that support HTML5 validation will check that the user has provided information in the correct format of an email address. Some smart phones also optimize their keyboard to display the keys you are most likely to need when entering an email address (such as the @ symbol).***
- ***type="url"A URL input can be used when you are asking a user for a web page address. Browsers that support HTML5 validation will check that the user has provided information in the format of a URL. Some smart phones also optimize their keyboard to display the keys you are most likely to need when entering a URL.***

# Lists, Tables and Forms
- ***List markers can be given different appearances using the list-style-type and list-style image properties.***
- ***Table cells can have different borders and spacing in different browsers, but there are properties you can use to control them and make them more consistent.***
- ***Forms are easier to use if the form controls are vertically aligned using CSS.***
- ***Forms benefit from styles that make them feel more interactive.***

# Events
***W hen you browse the web, your browser registers different types of events. It's the browser's way of saying, "Hey, this just happened." Your script can then respond to these events.***

## HOW EVENTS TRIGGER JAVASCRIPT CODE
1. **Select the element node(s) you want the script to respond to.**
2. **Indicate which event on the selected node(s) will trigger the response.**
3. **State the code you want to run when the event occurs.**

## THREE WAYS TO BIND AN EVENT TO AN ELEMENT
- **HTML EVENT HANDLERS**
- **TRADITIONAL DOM EVENT HANDLERS**
- **DOM LEVEL 2 EVENT LISTENERS**

## THE EVENT OBJECT
***When an event occurs, the event object tells you information about the event, and the element it happened upon.***

## EVENT DELEGATION
***Creating event listeners for a lot of elements can slow down a page, but event flow allows you to listen for an event on a parent element.***

## CHANGING DEFAULT BEHAVIOR
***The event object has methods that change: the default behavior of an element and how the element's ancestors respond to the event.***

> **Note: The most commonly used events are W3C DOM events, although there are others in the HTMLS specification as well as browser-specific events.**