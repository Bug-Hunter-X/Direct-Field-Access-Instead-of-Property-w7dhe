# Direct Field Access Instead of Property in C#

This example highlights a potential issue in C# where a class's field is accessed directly from within a method instead of going through the property. This can lead to unexpected behavior if the property has validation or other logic in its setter.

## Problem
The `MyMethod` function directly modifies the `_myField` field, bypassing the property's setter.

## Solution
The solution involves modifying `MyMethod` to use the property `MyProperty` instead of directly accessing the field `_myField`.