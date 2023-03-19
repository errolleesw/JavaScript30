# Javascript Event Capture, Porpagation and Bubbling - Follow along

Link: https://www.youtube.com/watch?v=F1anRyL37lE

## Key Learnings

- **Event bubbling**: When an event is triggered on an element, the event will propagate (or "bubble up") through its parent elements all the way up to the document. This means that if you click on a child element within a parent element, the parent element (and all of its ancestors) will also receive the event.

- **Event capture**: The `addEventListener()` method has an optional third parameter called `useCapture` that allows you to reverse the order of event propagation. If `useCapture` is set to `true`, the event will be triggered on the parent elements first before propagating down to the child elements. By default, `useCapture` is set to `false`.

- **`stopPropagation()`**: When an event is triggered on an element, you can use the `stopPropagation()` method to prevent the event from propagating further up the DOM tree. This means that the event will not be triggered on any parent elements above the current element.

- **`once` option**: The `addEventListener()` method has an optional `{ once: true }` option that allows you to listen for a particular event only once. Once the event is triggered, the event listener will be removed automatically. This is useful in situations where you only want a particular event to be handled once, such as a "checkout" button that should only be clicked once.
