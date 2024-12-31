# Tcl proc: Missing Braces in Procedure Body

This example demonstrates a subtle error in Tcl where missing braces in a procedure's body can lead to unexpected behavior.  The `badproc` procedure below is incorrectly defined, and will not work as expected.

## Bug

The issue lies in the `if` statement within the procedure.  The correct syntax requires braces around both the 'true' and 'false' branches. Without them, only the first command following the conditional is executed. 

**bug.tcl** contains the code demonstrating the bug.