# Unexpected Behavior with Loose Comparison and NaN in JavaScript

This repository demonstrates a subtle bug in JavaScript related to loose comparison (`==`) and the handling of `NaN` (Not a Number).

## The Bug
The `foo` function intends to classify inputs as negative, zero, or positive. However, due to JavaScript's loose comparison, `NaN` is incorrectly treated as a positive number.

## The Solution
The solution involves using strict comparison (`===`) to avoid the unexpected behavior caused by type coercion.  The corrected function explicitly handles `NaN` using `isNaN()`.

## How to Reproduce
1. Clone this repository.
2. Open `bug.js` to see the buggy code.
3. Run `bug.js` using Node.js (or your preferred JavaScript runtime).
4. Observe the unexpected output for the `NaN` input.
5. Open `bugSolution.js` to see the corrected code.
6. Run `bugSolution.js` to see the corrected output. 