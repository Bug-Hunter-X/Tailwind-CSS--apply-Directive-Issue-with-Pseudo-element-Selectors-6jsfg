# Tailwind CSS @apply Directive Issue with Pseudo-elements

This repository demonstrates a bug where Tailwind CSS's `@apply` directive doesn't correctly apply styles to pseudo-elements (::before, ::after) when used within a class that contains pseudo-element selectors.

## Bug Description
The `@apply` directive, when applied to a class containing pseudo-element selectors, fails to correctly apply the styles to the pseudo-elements. This often results in the pseudo-element having no styles applied or unexpected styling inconsistencies.

## Reproduction
1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe the missing or incorrectly styled pseudo-element.

## Solution
The solution is demonstrated in `bugSolution.html`. Instead of using the `@apply` directive directly on classes with pseudo-element selectors, apply the styles directly within the class definition itself.