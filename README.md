# JAVASCRIPT-CallbackFunctions

|header|header|
|----|----| 
|||

Functions are objects <br>
Objects can be passed into functions as parameters <br>
SO, functions can pass as parmeters into functions and then called inside <br>
A function that takes another function as a parameter and calls it inside is called a CALLBACK<br>
The function passed in as a parameter to another function is a CALLBACK FUNCTION<br>
JavaScript runs in sequence top down<br>
Sometimes JavaScript must run non sequencially but AFTER SOMETHING HAS HAPPENED. (or asynchronously) <br>
Callbacks helps code run asychronously<br>
#### Create a CallBack

Eg. SetTimeout function is a callback function. Which calls a function after a certain amount of time has passed (or AFTER SOMETHING HAS HAPPENED) <br>
setTimeout(message,3000) ---> here the function message is being called afer 3s (3s is the AFTER SOMETHING ELSE HAS HAPPENED).

##### Anonymous function          function(){....code to execute}

      setTimeout(function() {  
          console.log("This message is shown after 3 seconds");
      }, 3000);
##### Arrow function      () -> {....code to execute}

      setTimeout(() => { 
          console.log("This message is shown after 3 seconds");
      }, 3000);

##### JavaScript is event driven so we use callbacks functions for event declarations <br>

Eg. What if we want users to see a message when a button is clicked.
1st We have the html button
`<button id="callback-btn">Click here</button>`
2nd We select the button with its ID and add an event listener with the addEvenlistener method and its 2 parameters
`.addEventListener(eventType, callback function)`

      document.queryselector("#callback-btn")
      .addEventListener("click", function() {    
        console.log("User has clicked on the button!");
    });
      
