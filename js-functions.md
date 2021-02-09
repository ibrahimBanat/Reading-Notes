# Funtions 

Browsers require very detailed instructions about what
we want them to do. Therefore, complex scripts can run
to hundreds (even thousands) of lines. Programmers use
functions, methods, and objects to organize their code. 

## What is the function 

Functions let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of statements).

### A basic function 


``` 
var msg = 'Sign up to recive out newsletter for 10% off!';

function updateMessage() {
    var el = document.getElementById('message');
    el.textContent = msg;
}
updateMessage();
```

### Declearing a function

To create a function, you give it a name and then write the statements needed to achibe it's task inside the curly braces. This known as a **function declaration**.
![](img/fucntion.PNG)


### Calling a function 

Having declared the function, you can excute all of the statements between it's curly braces with just one line of cide.
this is known as calling the function.

![](img/invoke.PNG)

### Declaring a Functions that need information
SomeTimes a function needs specific information to perform it's task.

In such cases, when you declare the function you give it **arameter**.

![](img/param.PNG)

- Arguments as values:
    ```
    getArea(3,5);
    ```

- Arguments as Variables 
    ```
    wallWidth = 3;
    wallheight = 5; 
    getArea(wallWidth, wallHieght);
    ```

### Getting a single value out of funtion 

Some function return information to the code that called them. For example, when they perform a calculation, they return the result.

```
function calcualteArea(width, height) {
    var area = width * height;
    return area;
}
var wallOne = calculateArea(3, 5);
var wallTwo = calculateArea(8, 5);
```


### Getting a multiple values out of function 

function can return more than one value using array. 
for example, this function calculates the area and the voulme of a box. 

``` 
function getSize(width, height, depth) { 
    var area = width * height;
    var volume = width * height * depth;
    var sizes = [area, volume];
}
var areaOne = getSize(3, 2, 3)[0];
var volumeOne = getSize(3, 2, 3)[1];





