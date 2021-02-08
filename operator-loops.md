## Decisions & Loops 

There are often several places in a script where decisions are made that determine which lines if code should be run next. Flowcharts can help you plan for these occasions.

![](img/lopps.PNG)

## Compariosn operators

you can evaluate a situation by comparing one value in the script to what you expect it might be. the result will be boolean: **true** or **false**.

|     ==      |     !=      |
| ----------- | ----------- |
| Is equal to | Is not equal to |

- Is Equal To:

    This operator compares two values(Numbers, Strings or Booleans) to see if they are the same.

    `'Hello'` == `'Goodbye'` return false, becasue they are not the same data type and value are the same. 

- Is Not Equal to:

    This operator compares two values(Numbers, Strings or Booleans) to see if they are not the same.

    `'Hello'` != `'Goodbye'` returns true because they are not the same.


|     ===     |     !==     |
| ----------- | ----------- |
| Strict equal to | Strict not equal to |


- Strict equal to: 

    This operator compares two values to check that both the data types and value are the same.

    `'3'` === `3` return false because the are not the same data type or value.

- Strict not equal:

    This operator compares two values to check that both the data type and value are not the same.

### Structuring comparison operators 

In any condition, there is usually one operator and two operands.The opernads are placed on each side of the operator. They can be values or variables. You can often see expressions enclosed in brackets.


![](img/comparison.PNG)

The enclosing brackets are important when the expression used as a condition in a comparison operator. But when you are assining a value to a variable, they are not needed.


## Logical operators 

Comparison operators usually return single values of `true` or `false`.
Logical operators allow you to compare the results of more than one comparison operator.

![](img/logical.PNG)

In this one line of code are three expressions, each of which will resolve to the value `true` or `false`.

The expressions on the left and the right both use comparison operators, and both return `false`.

The third expression uses a logical operator(rather than a comparison operator). The logical AND operator checks to see whether both expression on either side of it return `true`.

- Logical AND ( && ):

    ```
    ((2 < 5 ) && (3 >= 2))
    ```
    returns `true`

If both expressions evaluate to `true` the the expressions returns `true`. if just one of these returns `false`, then the expressions will return `false`.

```
true && true returns true
true && false returns false
false && true returns false
false && false returns false
```

- Logical OR ( || ):

    ```
    ((2 < 5 ) && (2 < 1))
    ```
    return true

This operator tests at least ine condition.


If either expressions evaluate to `true` the the expressions returns `true`. if both of these returns `false`, then the expressions will return `false`.

```
true || true returns true
true || false returns true
false || true returns true
false || false returns false
```


- Logical NOT( ! ):

    This operator takes a single Boolean value and inverts it.

    ```
    !(2 < 1)
    ```
    returns true

The reverse the state of an expression. if it was `false`, it would return `true`. if the staement was `true`, it would return `false`.

```
!true returns false
!false returns true
```


## Loops 

Loops check a condition. if it returns `true`, a code block will run.
Then the condition will be checked again and if it still returns `true`, the code clock will run again. it repeats until the condition returns `false`.

![](img/for.PNG)

There are three common types of loops: 

#### FOR 

if you want ti run code a specific number of times, use a for loop.
in a for loop, the condition is usually a counter which is used ti tell how many times the loop should run.

#### WHILE 

If you do know how manu time the code shoukd run, you cac use a while loope. Here the condition can be something other than a counter, and the code will continue to loop for as long as the condition is true.


#### DO WHILE 

the do ... while loop is very similir to the while loop, but has one key difference: it will always run the statements inside the block at least once, even if the condition evaluates to false.

### Loop counter 

a for loop uses a counter as condition. This instructs the code to reun a specified number of times.
Here you can see the condition is made up of three statements: 

- Initialization 

    create a variable and set it to 0.

    ```
    var i = 0;
    ```

- Condition

    The loop should continue to run until the counter reaches a specified number.

    ```
    i < 10;
    ```

- Update 

    Every time the loop has run the statement in the curly braces, it adds to the counter.

    ```
    i++
    ```

## Using while Loops 
Here is an example of a while loop. it writes out hte 5 times table. Each time the loop is run, another calculation is written into the variavle called **msg**.
```
var i = 1;      //Set counter to 1
var msg = '';   //Message

// Store 5 times table in a variable 
while (i < 10){
    msg += i + ' x 5 = ' + (i * 5) + '<br>';
    i++;
}
document.getElementById('answer').innerHTML = msg;
```



