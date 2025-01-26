# CSS Specificity and Inheritance Issue

This repository demonstrates a subtle but important issue related to CSS specificity and the `inherit` keyword. The problem arises when trying to inherit a property from a parent element when more specific selectors are involved.

## The Problem

The `inherit` keyword in CSS is designed to inherit a property value from the parent element. However, in cases involving complex selectors and specificity, the inherited value might not be what you expect. The example provided shows this unexpected behavior.

## Setup

1. Clone this repository.
2. Open `bug.css` to see the problematic CSS code.
3. Open `bugSolution.css` to see the solution.

## Solution

To solve this, use explicit selectors and avoid the ambiguity caused by specificity conflicts.  Explicitly setting the color on the most specific selector (`.container p.special`) makes the inheritance work as expected.