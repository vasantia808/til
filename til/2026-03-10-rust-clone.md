# TIL: Rust clone() Method

**Date:** 2026-03-10

## What I Learned

Today I learned about the Rust .clone() method, which is used to create an independent duplicate.

## Basic Syntax

`let original_item = String::from("important text");
let cloned_item = original_item.clone();`

## Why It Matters

With the clone() method, you can create an independent copy that you can mutate without affecting the original. 
It is important to note that when you use the clone() method, you are creating a duplicate of both the heap 
and the stack, which can use up a lot more memory, depending on what you are cloning. Since performance cost 
can be affected, it is important to know when to borrow and when to clone. 

I learned the Rule of Thumb: "Always borrow until you have to clone".

## Resources

- [Rust Book](https://doc.rust-lang.org/book/ch04-01-what-is-ownership.html#ways-variables-and-data-interact-clone)
