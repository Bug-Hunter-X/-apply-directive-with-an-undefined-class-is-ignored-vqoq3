# @apply Directive with Nonexistent Class in Tailwind CSS

This repository demonstrates a subtle bug that can occur when using Tailwind CSS's `@apply` directive with a class that is not defined in your Tailwind configuration.

## The Bug
The `@apply` directive is a powerful feature that allows you to apply pre-defined utility classes to your components. However, if the class you're attempting to apply doesn't exist, it silently fails, resulting in unpredictable styling issues.

## Reproduction
1. Clone this repository.
2. Open `bug.html` in your browser. You'll observe that the text is not styled as expected.

## Solution
The solution involves ensuring that all classes used within the `@apply` directive are defined in your `tailwind.config.js` or `tailwind.config.cjs` file. 

See the `solution.html` for the corrected implementation.