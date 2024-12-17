# TypeScript Type Error: String element in number array

This code demonstrates a common type error in TypeScript that occurs when an array is expected to contain only numbers, but it contains a string element. This leads to a type error during compilation or runtime, depending on how strict the type checking is configured.

The bug is in the `combine` function, where the `arr2` array contains a string element ("6"). The function attempts to concatenate two arrays using the spread syntax.  TypeScript's type system detects the type mismatch and throws an error.

## Solution

The solution involves ensuring that both arrays passed to the `combine` function contain only numbers.  This can be done by ensuring the inputs are correctly typed, by adding runtime checks, or by using type guards.