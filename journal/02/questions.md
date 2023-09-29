# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > |let, var, const|

02. What is the definition of a function?

    > | it is a subprogram designed to perform a certain task. Functions return something, and if no return value is assigned, it will say undefined. Functions are executed when they are called.  |

03. What are the `SOLID` principles?

    > | single responsibility, open-closed, liskov substitution, interface segregation, and dependency inversion|

04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```

    > | delete array[2];|

05. Given these two objects: How could you add each to the others friends arrays?

    ```js
    let you = {
        name: "You",
        hair: true,
        friends: []
    }
    let them = {
        name: "Them",
        hair: false,
        friends: []
    }
    ```

    > |let newArray = you.concat(them);  |

06. Give an example of a JavaScript `Conditional`:

    > | if( 10%2 == 0){
    > console.log('success')
    > }|

07. What is the main difference between `parameters` and `arguments`?

    > | parameters are used when defining a function, and are the names created in the function. arguments are the values the function receives.  |

08. Instead of writing everything to the console, what is a better way to debug your code?

    > | setting breakpoints, using your developer tools|

09. What is the difference between a `primitive` value and a `reference` value?

    > | they are stored differently in memory|

10. Demonstrate a loop that prints the numbers between -100 and 100?

 
    > for( i = -100; i <= 100; i ++){
    > console.log(i)
    > }|
