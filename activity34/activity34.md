**Learning outcome:**

User should be able to identify problems where event bubbling can be utilised for better solutions
User should be able to implement event delegation by leveraging event bubbling

Note for the author who checks the solution: These above two learning outcomes could be combined together - it would be better as we leverage the event bubbling process to implement event delegation

**Activity:**

Create a list of products - product section where each product will have add, remove button.
such that when these buttons are clicked, product should be added in cart and removed from cart appropriately from list of carts - cart section. Try to do both the functionality by adding only a single event listener. Remember how the event bubbling process happens all the way up to root element starting from child element based on previous learnings.You should try to manage both add to cart / remove from cart essentailly from the parent product container.Try doing add to cart functionality first and extend it to removing the item from cart.

Note: Please refer the cart-add-remove-product image to see how it needs to be built for
more clartiy on UI. Please open the image with chrome browser.

**Screenshots:**

![cart-add-remove-product img](cart-add-remove-product.png)

Note for the author who checks the solution: If it feels hard to follow even after giving UI images and exact activity description, we can provide the bare bones, basic skeleton code to work on. it would be more better to follow through.

Hint: Think how you can distinguish between add to cart, remove from cart button element - id, className, custom data attributes etc. log the event object and check out properites that you can make use of in your code. Handling cases where trying to add product on already added item and removing already removed item / or non-existing item from cart is not necessary. You can try doing it as bonus task

Note for the author who checks the solution: We can explain how we leverage event bubbling by attaching a single event listener on parent which helped without having multiple listeners thereby memory efficient and how we delegated the different clicks - add to cart, remove from cart
