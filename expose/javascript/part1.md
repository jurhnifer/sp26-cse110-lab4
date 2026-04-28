1. By line 9, it will print 20.
2. By line 13, it will print 20.
3. There are still scoping issues, there's no block-scope. The var result is essentially a global variable. Because you can use var anywhere in the function, this can cause confusion since the result variable was only supposed to be inside of the curly braces blocks, not outside. The var variables can be used accidentally elsewhere that is not supposed to be used in.
4. By line 9, it will print 20.
5. This will throw an error, a ReferenceError. The let result is only visible inside the if, not outside of it.
6. The code returns a TypeError because there is an assignment to a constant variable. By rule, declared const variables cannot be reassigned. The variable is meant to never change.
7. Line 13 will not be reached because the function stops at line 9 due to the TypeError.