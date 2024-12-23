**Interview questions with answers:**

1.What is the different phases related to event propagation ?

Event propagation has three phases:

Capturing Phase: The event travels from the outermost ancestor to the target element.
Target Phase: The event reaches and is handled by the target element.
Bubbling Phase: The event bubbles up from the target element to the outermost ancestor.

2.How do you control the flow of the phases, bubbling and capturing ?

We can control the phase with the addEventListener method by setting the third argument to true (capturing) or false (bubbling) - default one.

3.What is the difference between event target and event currentTarget ?

event.target refers to the element that triggered the event (e.g., the clicked element).
event.currentTarget refers to the element the event listener is currently attached to.

**Curious questions with answers:**

1.Assume you have multiple event listeners on a single element with default behavior - bubbling phase.

If you want to stop propagation, you can use event.stopPropagation(). will this line be required in all event listener callbacks or not ?. Can we remove writing event.stopPropagation() in all event listener callbacks ? How would you stop the propagation from happening if you can't use it more than once ?

We can stop the event propagation and also prevent other listeners from being triggered on the same element, we can use event.stopImmediatePropagation(). This will stop both propagation and prevent other event listeners from being called.

2.Do all events work on bubbling phase ?.
How you can find say "blur" whether the event can bubble or not ?

Yes most events like click, keydown, and mousemove go through the capturing and bubbling phases.
Some events like focus, blur, mouseenter, and mouseleave do not follow the bubbling or capturing phases.

You can search in the MDN docs for any event that you need to check for. It will be mentioned there if it is not supported. usually, in first three sentences.

Link: https://developer.mozilla.org/en-US/docs/Web/API/Element/blur_event

![blur event mdn doc preview img](blur-event-mdn.png)
