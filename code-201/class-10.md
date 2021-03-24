## **Error Handling & Debugging**
### EXECUTION CONTEXT
Every statement in a script lives in one of three
execution contexts:
* GLOBAL CONTEXT :
Code that is in the script, but not in a function.
There is only one global context in any page.
    * FUNCTION CONTEXT
Code that is being run within a function.
Each function has its own function context.
    * EVAL CONTEXT (NOT SHOWN)
Text is executed like code in an internal function.

* VARIABLE SCOPE :
The first two execution contexts correspond with the
notion of scope
    * GLOBAL SCOPE
If a variable is declared outside a function, it can
be used anywhere because it has global scope.
    * FUNCTION-LEVEL SCOPE
When a variable is declared within a function,
it can only be used within that function.

### **EXECUTION CONTEXT & HOISTING**
There are two phases
of activity:
* PREPARE
    * The new scope is created.
    * Variables, functions, and arguments are created.
    * The value of the this keyword is determined.
* EXECUTE
    *  Now it can assign values to variables.
    * Reference functions and run their code.
    * Execute statements  . 
### **ERROR OBJECTS CONTINUED**
* Syntax Error :SYNTAX IS NOT CORRECT
* ReferenceError : VARIABLE DOES NOT EXIST
* EvalError :
INCORRECT USE OF eval() FUNCTION
* URI Error :
INCORRECT USE OF URI FUNCTIONS
* Type Error :
VALUE IS UNEXPECTED DATA TYPE
* RangeError :
NUMBER OUTSIDE OF RANGE
* Error:
GENERIC ERROR OBJECT
* NaN:
NOT AN ERROR

### There are two things you can do with the errors:
* DEBUG THE SCRIPT TO FIX ERRORS
* HANDLE ERRORS GRACEFULLY