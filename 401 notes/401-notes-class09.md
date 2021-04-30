# Class-09: Stacks and Queues:

## Stack:

- a data structure that consists of linked nodes that follows _first in, last out_ convention.
- think of it like pancakes. the pancake on top of the stack was the last one to be added, and will be the first one to get eaten.

  - Push: Nodes or item is put into the the stack
  - Pop: Removes that last item to be added to the stack
  - Top: the head of the stack
  - Peek: to view the value of the top item in the stack
  - isEmpty: returns true if the stack is empty. false if otherwise.

- All these methods can and do operate at `O(1)`.

## Queue:

- a data structure that behaves kind of like a stack, but it instead acts on _first in, first out_

  - Enqueue: adding node to the queue.
  - Dequeue: removing node from the queue. **will raise exception if the queue is empty**
  - Front: the first node in the queue.
  - Rear: the tail of the stack.
  - Peek: returns that value of the first item in the queue
  - isEmpty: will return true if the queue is empty, false otherwise.

    - also operates on `O(1)` time
