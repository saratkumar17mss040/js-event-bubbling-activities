**Learning outcome:**

User should be able to prevent event bubbling using event.stopPropagation()

Note for the author who checks the solution: We can give our solution for the activity 1 and we can ask the
learners to build on top of it.

**Activity:**

As you have done the first activity, while doing subacitivity 1.3 before,
(i.e),

Subactivity 1.3: click on overlay wrapper after opening the modal and observe the sequence in which the logs are printed.
The behavior would have been that after clicking on the overlay wrapper - the modal is closed. This was the explicit acivity that was asked to do initially.

Now, after checking - Ideally, we want the modal to be closed only when modal inside button is clicked. Please, update the code such that it doesn't get closed when overlay or modal content is clicked.

**Skeleton code:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Event Bubbling with Modal - Acitivity - 1</title>
    <style>
      .overlay {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: rgba(0, 0, 0, 0.5);
        display: flex;
        justify-content: center;
        align-items: center;
      }
      .modal {
        background: white;
        padding: 20px;
        border-radius: 5px;
        width: 300px;
        text-align: center;
      }
    </style>
  </head>
  <body id="body">
    <button id="open-modal-btn">Open Modal</button>

    <div id="modal-overlay" class="overlay" style="display: none">
      <div id="modal-content" class="modal">
        <h3>Modal Content</h3>
        <button id="btn-inside-modal">Click Inside Modal</button>
      </div>
    </div>

    <script>
      // write your solution here
    </script>
  </body>
</html>
```

Make sure, to check all the sequence similar to how we had the subacitivties
in activity 1. do all the subactivities of Activity 1 and check the sequence of
logs. make use of style.diplay property for it. it would be more better to
follow through.

Additional link on how to stop event propagation: https://developer.mozilla.org/en-US/docs/Web/API/Event/stopPropagation

Note for the author who checks the solution: We can explain the
solution, on how the event.stopPropagation() worked while clicking on the
overlay, the log for body element is not printed, thereby stopping it from
propagation.

Solution: [link](index.html)

Add on section based on given feedback:

activity2.md

Expected learning outcome: User should be able to prevent event bubbling using event.stopPropagation()

Activity: "we want the modal to be closed only when modal inside button is clicked. Please, update the code such that it doesn't get closed when overlay or modal content is clicked"

Observation: Even after commenting out the "event.stopPropagation();" in the overlay event listener, clicking anywhere other than the inner button doesn't close the modal. What is the need for "event.stopPropagation();", then, for this use case?

For this, as per the observation i have reframed the question:

"we want the modal to be closed only when modal inside button is clicked. Please, update the code such that it doesn't get closed when overlay or modal content is clicked and also make sure when overlay and modal content is clicked, the event should not bubble up all the way to the body"
which means it should not log "Body clicked" for any action.

Through this, the need for event.stopPropagation() is must.

