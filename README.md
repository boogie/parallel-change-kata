# Parallel Change challange

"Making a change to an interface that impacts all its consumers requires two thinking modes: implementing the change itself, and then updating all its usages. This can be hard when you try to do both at the same time, especially if the change is on a PublishedInterface with multiple or external clients." - read more about it at [ParallelChange](https://www.martinfowler.com/bliki/ParallelChange.html) from martinfowler.com, or at [Parallel Change (Parallel Design)](https://blog.jakubholy.net/wiki/development/parallel-design-parallel-change/) from jakubholy.net.

You should break the change into three distinct phases:
- *expand* - add the new design without breaking the old,
- *migrate* - switch over to using the new design,
- and *contract* - write tests for the new features.

The challange and the JavaScript code is from the [Parallel Change Kata](https://kata-log.rocks/parallel-change-kata).

## Your Task

1) clean up the Field/ShoppingCart class, check the relevant tests, understand the code.
2) currently it is handling one price, *the goal is to handle multiple*.
3) if you have time left, add handling product names, and a method to query the full shopping cart contents.

Tests have already been written, as you go forward, you should modify and expand them.

## Rules

The tests must not be red at any time. No compile-errors, no failures. (The only exception is for a few seconds while you write a single line of code.)
