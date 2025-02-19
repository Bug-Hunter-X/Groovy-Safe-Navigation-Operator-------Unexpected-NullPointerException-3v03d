# Groovy Safe Navigation Operator (?.): Unexpected NullPointerException

This example demonstrates a potential pitfall when using Groovy's safe navigation operator (`?.`). While designed to prevent `NullPointerExceptions`, improper usage can still lead to unexpected behavior if not carefully considered.

The `bug.groovy` file shows how a seemingly safe approach can still throw a `NullPointerException` when dealing with potentially null values. The `bugSolution.groovy` offers a solution that clearly handles null cases.

## How to Reproduce

1. Run the `bug.groovy` script.
2. Observe the `NullPointerException` thrown by the `MyOtherClass` method.

## Solution

The `bugSolution.groovy` provides a corrected version where null input is explicitly checked and handled before attempting to call `toUpperCase()`.

This showcases the importance of carefully considering null handling even when using Groovy's safe navigation operator.