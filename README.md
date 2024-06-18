# JAVASCRIPT-CallbackFunctions


Functions are `OBJECTS` <br>
Objects can be passed into functions as parameters <br>
SO, functions pass as parmeters into other functions and then called from inside <br>
`CALLBACK` - A function that takes another function as a parameter and then called <br>
A passed in function (as parameter) to another function is a CALLBACK FUNCTION<br>

#####JavaScript runs in sequence top down<br>
Sometimes JavaScript must run non sequencially but AFTER SOMETHING HAS HAPPENED. (or asynchronously) <br>
Callbacks helps code run asychronously<br>

#### Create a CallBack

Eg. SetTimeout function is a callback function.<br> 
It calls a function after a certain amount of time has passed (AFTER SOMETHING HAS HAPPENED) <br>
setTimeout(message, 3000) ---> Here, function message is called ater 3s (3s is the AFTER SOMETHING ELSE HAS HAPPENED).<br>

##### Anonymous function          function(){....code to execute}

      setTimeout(function() {  
          console.log("This message is shown after 3 seconds");
      }, 3000);
##### Arrow function      () -> {....code to execute}

      setTimeout(() => { 
          console.log("This message is shown after 3 seconds");
      }, 3000);
##### Function expression

     const message = function() {  
          console.log("This message is shown after 3 seconds");
      }
 
      setTimeout(message, 3000);

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
      
