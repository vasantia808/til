# TIL: Rust Troubleshooting

**Date:** 2026-03-15

## What I Learned

When troubleshooting code that contains multiple Rust compile errors, 
you should do a top->down approach. This is important because sometimes
when you fix one error, some of the ones below it may also go away.

**General Troubleshooting Approach**
1. Read the first error message, looking for location of the error and
any suggestions on how to correct it.
2. Fix the one error
3. Recompile before touching anything else
4. Repeat

Rust has compiler errors with a code that looks like `E0308`. You can use
the built-in tool that will give you a detailed explanation of the error 
and examples.

## Basic Syntax

`rustc --explain E0308`

## Why It Matters

Following the General Troubleshooting Approach seems like it may take longer,
but it actually can save you time. The `rustc --explain <error>` gives you more
information about the error presented and is helpful, especially if you do 
not fully understand the inline compiler error messages.

## Resources

- [Rust Error Codes](https://doc.rust-lang.org/error_codes/)
