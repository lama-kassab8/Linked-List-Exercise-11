# LeetCode - Add Two Numbers

**Problem:** [Add Two Numbers](https://leetcode.com/problems/add-two-numbers/)

## Problem Description

You are given two **non-empty** linked lists representing two non-negative integers.  
The digits are stored in **reverse order**, and each of their nodes contains a **single digit**.

Add the two numbers and return the **sum as a linked list**.

You may assume the two numbers do not contain any leading zero, except the number 0 itself.


## Approach

- Use two pointers `p1` and `p2` to walk through `l1` and `l2`.
- Add corresponding values from the lists along with a `carry`.
- Use a `dummy` node to build the result list without special cases.
- Use `current.next = ListNode(updated_sum)` to link each new digit node.
- Return `dummy.next` to skip the initial placeholder.
