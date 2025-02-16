# PHP Loose vs. Strict Comparison: A Subtle Source of Errors

This repository demonstrates a common error in PHP: the misuse of loose (`==`) versus strict (`===`) comparison operators.  Loose comparison can lead to unexpected behavior and make debugging difficult.

## The Problem
PHP's loose comparison (`==`) performs type juggling, converting values to a common type before comparing.  This can mask errors when comparing values of different types.

## The Solution
Always use strict comparison (`===`) unless you specifically intend to allow type coercion.  This leads to more predictable and maintainable code.

## How to Use
1. Clone this repository.
2. Run `bug.php` to see the unexpected behavior of loose comparison.
3. Run `bugSolution.php` to see the corrected behavior using strict comparison.

This example highlights a subtle, yet pervasive, issue in PHP programming that can be easily avoided with careful attention to detail.