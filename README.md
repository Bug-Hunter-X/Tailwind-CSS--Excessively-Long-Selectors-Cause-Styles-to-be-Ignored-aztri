# Tailwind CSS: Excessively Long Selectors Bug

This repository demonstrates a bug that can occur in Tailwind CSS projects when class names become excessively long, exceeding browser limits and causing styles to be ignored. This is especially problematic with complex responsive designs and many style modifiers.

## Problem

Tailwind's utility-first approach is fantastic for rapid development, but combining numerous modifiers (e.g., `md:hover:bg-blue-500`) or applying many utilities to a single element can create exceptionally long CSS selectors.  Browsers have limits on selector length; exceeding this limit causes the browser to ignore the associated styles.

## Solution

The solution involves optimizing class names and potentially using techniques like CSS modules or a CSS preprocessor to manage styles more efficiently. This example shows how refactoring and using CSS variables can be helpful. 

## Reproduction

1. Clone this repository.
2. Open `bug.html` in your browser.  You will observe that some styles are missing.
3. Open `bugSolution.html` to see the improved version with optimized class names.
