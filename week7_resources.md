# Dynamic Programming from First Principles

Before starting Dynamic Programming, make sure you are **comfortable with recursion and backtracking**.

By "comfortable", I mean you should be able to:

* Draw and understand a recursion tree.
* Solve standard recursion/backtracking problems.
* Naturally think of recursive solutions before optimization.
* Analyze the time complexity of recursive solutions.

If you are not confident with these, **please don't start DP yet**. DP is simply an optimization over recursion.

## Resources

### 1. DP from First Principles (Primary Playlist)

https://www.youtube.com/watch?v=G-uriCpjSOA&list=PLAj_13N2fk-RA6wvOUmWOyUeL9zmWFJoI

* Follow **one lecture per day**.
* You can **skip the last lecture** for now.

If you prefer reading over watching lectures, the **Dynamic Programming** chapter in the CSES Competitive Programmer's Handbook is an excellent resource:

https://cses.fi/book.pdf

---

### 2. Standard DP Practice (CSES)

https://www.youtube.com/watch?v=nEEROBg1kbg&list=PLcXpkI9A-RZI-xF76L0sZq_u-k_yHz8pd

Complete the standard CSES DP problems alongside the lectures (or after reading the chapter).

---

### 3. Additional Practice (NeetCode 250)

https://neetcode.io/practice/practice/neetcode250

Use this to practice standard DP problems once you're comfortable with the basics.

## How to Practice

For every problem:

1. Spend time trying to solve it on your own.
2. If you're stuck, look at the solution.
3. Understand **why** the solution works instead of memorizing it.

I am **not assigning extra Codeforces DP problems** right now. If you finish the CSES set and want more practice, let me know and I'll suggest a good list.

## Most Important Advice

**Do NOT memorize DP.**

For every problem, ask yourself:

* What is the **state**?
* Why is this state sufficient?
* What does `dp[state]` represent?
* How do we transition from one state to another?
* Why is this transition correct?

Understanding the **state definition** and the **transition** is far more important than remembering a particular solution.

> **Disclaimer:** While you should avoid memorizing solutions, you **do need to be familiar with standard DP patterns**. Knowing these patterns will help you recognize and solve more complex, non-standard DP problems later.
