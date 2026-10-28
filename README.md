# Task 10: JavaScript Event Loop

Output:
1 start
4 end
3 promise
2 timeout

Explanation:
JavaScript executes synchronous code first.
Promise callbacks run after synchronous code.
The setTimeout callback runs after the Promise callback.
