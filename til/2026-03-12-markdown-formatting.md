# TIL: Markdown Formatting

**Date:** 2026-03-12

## What I Learned

Today I learned that when you use comments inside of a code block in Markdown, any command keywords will still be 
identified as a command and not as part of the comment, so the visual formatting will not display correctly.

## Basic Syntax

For example, each of the following displays differently. The changes can be seen in the raw file view.

```cmd
hostname
# Find hostname
```

```cmd
hostname
# Display hostname
```

```cmd
hostname
# Display name of the host
```

In the first code block, 'Find' and 'hostname' are both flagged as keywords and, therefore, displayed in red.
In the second block, I changed 'Find' to 'Display' and it displays in white. Now only 'hostname' is flagged as a keyword/code in red.
In the third block, I changed the text for 'hostname' to 'name of the host' and now nothing is flagged and 
now the whole thing displays as a comment in white.

## Why It Matters

This is just something that I didn't know about and is good to know so that I can keep 
consistent formatting within my files.
