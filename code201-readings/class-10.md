## Eroor handling and debugging 

JavaScript can be hard to learn and everyone makes
mistakes when writing it. This chapter will help you learn
how to find the errors in your code. It will also teach you how
to write scripts that deal with potential errors gracefully. 

## ORDER OF EXECUTION

To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run.

## EXECUTION CONTEXTS

he JavaScript interpreter uses the concept of execution **contexts**.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope. 

* EXECUTION CONTEXT

    Every statement in a script lives in one of three
execution contexts:


    1. GLOBAL CONTEXT

        Code that is in the script, but not in a function.
        There is only one global context in any page. 
    2. FUNCTION CONTEXT

        Code that is being run within a function.
        Each function has its own function context.
    3. EVAL CONTEXT

        Text is executed like code in an internal function
        called eva l {) (which is not covered in this book).


## HOW TO DEAL WITH ERRORS

Now that you know what an error is and how the browser treats them,
there are two things you can do with the errors. 

## A DEBUGGING WORKFLOW

Debugging is about deduction: eliminating potential causes of an error.
Here is a workflow for techniques you will meet over the next 20 pages.
Try to narrow down where the problem might be, then look for clues.

## BROWSER DEV TOOLS & JAVASCRIPT CONSOLE 

The JavaScript console will tell you when there is a problem with a script,
where to look for the problem, and what kind of issue it seems to be.

The JavaScript console is just one of several developer tools that are
found in all modern browsers.

## BREAKPOINTS 
You can pause the execution of a script on any
line using breakpoints. Then you can check the
values stored in variables at that point in time.

## STEPPING THROUGH CODE

If you set multiple breakpoints, you can step
through them one-by-one to see where values
change and a problem might occur.

## CONDITIONAL BREAKPOINTS

You can indicate that a breakpoint should be
triggered only if a condition that you specify is
met. The condition can use existing variables. 

## HANDLING EXCEPTIONS

- TRY

    First, you specify the code
    that you think might throw an
    exception within the try block.

    If an exception occurs in this
    section of code, control is
    automatically passed to the
    corresponding catch block.

    The try clause must be used in
    this type of error handling code,
    and it should always have either
    a catch, fi na 1 ly, or both.

    If you use a continue, break, or
    return keyword inside a try, it
    will go to the f i na 11 y option. 

- CATCH

    If the try code block throws an
    exception, catch steps in with an
    alternative set of code.

    It has one parameter: the error
    object. Although it is optional,
    you are not handling the error if
    you do not catch an error.

    The ability to catch an error can
    be very helpful if there is an issue
    on a live website.

    It lets you tell users that
    something has gone wrong
    (rather than not informing them
    why the site stopped working). 

- FINALLY

    The contents of the fi na 11 y
    code block will run either
    way - whether the try block
    succeeded or failed.

    It even runs if a return keyword
    is used in the try or catch block.
    It is sometimes used to clean up
    after the previous two clauses.

    These methods are similar
    to the `.done()`, `. fail()`, and
    . a 1 `ways()` methods in jQuery.
    You can nest checks inside each
    other (place another t ry inside a
    catch), but be aware that it can
    affect performance of a script. 

## THROWING ERRORS 
If you know something might cause a problem for your script, you can
generate your own errors before the interpreter creates them. 

```
throw new Error('message') ;
```


## DEBUGGING TIPS 
Here are a selection of practical tips that you
can try to use when debugging your scripts.

- ANOTHER BROWSER 

    Some problems are browserspecific. Try the code in another
    browser to see which ones are
    causing a problem.

- ADD NUMBERS

    Write numbers to the console
    so you can see which the items
    get logged. It shows how far your
    code runs before errors stop it.

- STRIP IT BACK 

    Remove parts of code, and strip
    it down to the minimum you
    need. You can do this either by
    removing the code altogether, or
    by just commenting it out using
    multi-line comments: 
    ```
    /* Anything between these
    characters is a cofllllent */
    ```

## Summary

- If you understand execution contexts (which have two
stages) and stacks, you are more likely to find the error
in your code.
- Debugging is the process of finding errors. It involves a
process of deduction.
- The console helps narrow down the area in which the
error is located, so you can try to find the exact error.
- JavaScript has 7 different types of errors. Each creates
its own error object, which can tell you its line number
and gives a description of the error.
- If you know that you may get an error, you can handle
it gracefully using the try, catch, finally statements.
Use them to give your users helpful feedback.