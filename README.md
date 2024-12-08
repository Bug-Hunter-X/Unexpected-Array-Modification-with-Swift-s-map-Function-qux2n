# Unexpected Array Modification with Swift's map Function

This example demonstrates a potential misunderstanding regarding Swift's `map` function.  The `map` function in Swift creates a *new* array containing the transformed elements. It does *not* modify the original array.  The bug arises from an assumption that the original array is modified in place. 

## Bug Description
The code uses the map function to double the numbers in an array. A common misconception is that `map` directly modifies the source array.  This is incorrect; the map function returns a *new* array.