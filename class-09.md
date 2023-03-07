# Class 9 notes

Forms can make a website interactive so that a user can send data to the web page and make things change based on what they inputted.

## HTML forms

1. Forms are important because they are one of the main ways for users to interact with a website. They can enter data and send it to the page/server so that something can be done with the information.
2. Some key things to keep in mind about user experience with forms is that you don't want to piss off users by asking for too much information so you want to make sure you only ask for what you need from them. It can also help users if you use the ```<fieldset>``` tag to group the elements in the form because it helps the visual grouping of the elements in the form and the screen readers when reading your page.
3. Some key form elements:
    1. ```<fieldset>``` to group the elements in a form for better UX.
    2. ```<legend>``` describes the purpose of the fieldset it's inside. It's basically a title.
    3. ```<input>``` creates an input where a user can type in or select data that gets sent. It can be a textbox, checkbox, radio button, or some other stuff.
    4. ```<label>``` A title for the input it is placed with (helps screen readers).
    5. ```<button>``` A way to submit the data that you input into the form.

## Learn JS

1. Events are something that listens for an action/event that a user or a web page does and when the user or the page does that action, then something happens (whatever you program to happen). There are a lot of different types of events like a click event, a submit event, a keyboard event like if you press the up or down keys, a load event, and some others. So, for example, if you want the page to turn red when a user clicks a button, you can create an event that waits for a user to click the button and then turns the page red when they do.
2. When using ```addEventListener()``` make sure to use the arguments: what type of event (in quotes) and then the event handler.
3. The event object is an object that is automatically passed into the event handler function. You can use the event object to access the event target (the element the event occurred on). This way you can collect the data the user inputted into the input element.
4. Event bubbling I believe is when you add an event handler to the parent element of the button or whatever you're trying to create an event with. It makes it so that if the user clicks (or whatever event type you have set) anything in the parent element the event handler will run. If you put event listeners on an element, the parent of that element, and the parent of THAT element, the innermost (most nested) element is going to run its' event handler first. Then the next innermost and so on. It's called 'bubbling up.' Event capturing is similar but it bubbles down so that the outermost element runs its' event handler first.

## Things I want to know more about
