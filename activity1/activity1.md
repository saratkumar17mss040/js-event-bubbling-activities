**Learning outcome:**

User understands the concept of event bubbling and how events propagate in the DOM

**Activity:**

Create a button to open a modal - open modal button, and a simple modal with overlay which is initially not displayed and create another button within the modal - button inside modal. add click event listeners for open modal button, button inside modal, overlay and modal - wrapper (div), body element and with callback functions logging which are clicked and make sure to toggle overlay display when opening the modal to show and when clicked on overlay it should hide the modal. make use of style.diplay property for it.

Note: Please refer the modal-closed and modal-opened images to see how it needs to be built for
more clartiy on UI. Please open the image with chrome browser.

**Screenshots:**

Modal opened state UI:

![modal-opened img](modal-opened.png)

Modal closed state UI:

![modal-closed img](modal-closed.png)

Note: Please make use of event bubbling nature to close the modal when button inside modal and modal content is clicked as well.

Hint: Event bubbling should be taken care in the parent element.

Subactivity 1.1: click on open modal button and observe the sequence in which the logs are printed.

Subactivity 1.2: click on button inside modal and observe the sequence in which the logs are printed.

Subactivity 1.3: click on overlay wrapper after opening the modal and observe the sequence in which the logs are printed.

Subactivity 1.4: click on modal content and observe the sequence in which the logs are printed.

Please make sure to clear your console logs after each click, to see the proper sequence and not get confused

Note for the author who checks the solution: If it feels hard to follow even after giving UI images and exact activity description, we can provide the bare bones, basic skeleton code to work on.

Note for the author who checks the solution: We can also add solutions to the subactivities
