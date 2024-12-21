**Learning outcome:**

User should be able to prevent event bubbling using event.stopPropagation()

Note for the author who checks the solution: We can give our solution for the activity 1 and we can ask the
learners to build on top of it.

**Activity:**

As you have done the first activity, while doing subacitivity 1.3 before,
(i.e),

Subactivity 1.3: click on overlay wrapper after opening the modal and observe the sequence in which the logs are printed.
The behavior would have been that after clicking on the overlay wrapper - the modal is closed.

Ideally, we want the modal to be closed only when modal inside button is clicked.
Please, update the code such that it doesn't get closed when overlay or modal content is clicked.

Make sure, to check all the sequence similar to how we had the subacitivties in activity 1. do all the subactivities of Activity 1 and check the sequence of logs. make use of style.diplay property for it. it would be more better to follow through.

Note for the author who checks the solution: We can explain the solution, on how the event.stopPropagation() worked while clicking on the overlay, the log for body element is not printed, therby stopping it from propagation.
