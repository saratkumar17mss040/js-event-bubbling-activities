**Learning outcome:**

User understands the difference between event bubbling and event capturing

**Activity:**

Create two div container - outer, middle and one inner button such that they are nested in structure and have id like below skeleton code.

**Eg:**

```html
<div id="outer">
  Outer div
  <div id="middle">
    Middle div
    <button id="inner-btn">Click me - inner btn</button>
  </div>
</div>
```

Add click event listeners to outer, middle div and inner button both in bubbling phase and capturing phase, you should basically have total of 6 event listener callback functions,

2 click event for outer div - capturing, bubbling phase,
2 click event for middle div - capturing, bubbling phase,
2 click event for inner button - capturing, bubbling phase.

Make sure to log on each callback function, event target id, currentTarget id

Note: Please refer this link for how to add event listeners in capturing phase: https://javascript.info/bubbling-and-capturing#capturing 

for to know difference between target vs currentTarget: https://www.jstips.co/en/javascript/difference-between-target-and-currentTarget

Now click on outer div, middle div, inner button and observe the sequence the logs are printed.
You can try turning on/off certain eventlistener that are in bubbling phase or capturing phase and observe the sequence of logs

Note for the author who checks the solution: we can come up with four exact sequences to do for the user later on and ask the user to check with our solution. later, we can explain how capturing phase works from ancestor element to child element. These four sequences could be part of subactivity 5.1,5.2,5.3,5.4.

This will help to solidify the flow of these phases. We can then mention some real world use case like form input field pre-processing.

I have added add on interview and curious questions as well in interview-questions.md file. Do take a look at it.

Solution: [link](index.html)

Interview questions link: [link](../interview-questions.md)


