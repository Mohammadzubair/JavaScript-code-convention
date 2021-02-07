# **JavaScript Style Guide:**

## **JavaScript Coding Conventions**
<br>

Coding conventions are **style guidelines for programming**. They typically cover:
<br>

### Naming and declaration rules for variables and functions.

- Naming and declaration rules for variables and functions.
- Rules for the use of white space, indentation, and comments.
- Programming practices and principles

### Coding conventions **secure quality:**


- Improves code readability
- Make code maintenance easier

Coding conventions can be documented rules for teams to follow, or just be your individual coding practice.

 ### **Variable Names:**
***
we use camelCase for identifier names (variables and functions).

### **All names start with a letter.**

> **like this**
<br>



    firstName = "Mohammad";
    
    lastName = "Zubair";

    price = 12;

    tax = 3.10;

    fullPrice = price + (price * tax);

<br>

### **Spaces Around Operators**
***

Always put spaces around operators ( = + - * / ), and after commas:

> **Examples:**
    



     var x = y + z;

     var values = ["Volvo", "Saab", "Fiat"];


<br>

### **Code Indentation**
***

Always use 2 spaces for indentation of code blocks:

> **Functions:**




    function toCelsius(fahrenheit) {
       return (5 / 9) * (fahrenheit - 32);
    }


<br>

### **Statement Rules**
***

General rules for simple statements:

- Always end a simple statement with a semicolon.

> **Examples:**



    var values = ["Volvo", "Saab", "Fiat"];

    var person = {
    firstName: "John",
    lastName: "Doe",
    age: 50,
    eyeColor: "blue"
    };


General rules for complex (compound) statements:

- Put the opening bracket at the end of the first line.
- Use one space before the opening bracket.
- Put the closing bracket on a new line, without leading spaces.
- Do not end a complex statement with a semicolon.


> **Functions:**



    function toCelsius(fahrenheit) {
       return (5 / 9) * (fahrenheit - 32);
    }


> **Loops:**



    for (i = 0; i < 5; i++) {
       x += i;
    }


> **Conditionals:**



    if (time < 20) {
      greeting = "Good day";
      } else {
      greeting = "Good evening";
    }

<br>

### **Object Rules**
***

General rules for object definitions:

- Place the opening bracket on the same line as the object name.
- Use colon plus one space between each property and its value.
- Use quotes around string values, not around numeric values.
- Do not add a comma after the last property-value pair.
- Place the closing bracket on a new line, without leading spaces.
- Always end an object definition with a semicolon.


> **Example:**



    var person = {*
        firstName: "John",
        lastName: "Doe",
        age: 50,
        eyeColor: "blue"
    };


Short objects can be written compressed, on one line, using spaces only between properties, like this:



    var person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};

<br>

### **Naming Conventions**
***

Always use the same naming convention for all your code. For example:

- Variable and function names written as **camelCase**.
- Global variables written in **UPPERCASE** (We don't, but it's quite common).
- Constants (like PI) written in **UPPERCASE**.

Should you use **hyp-hens, camelCase,** or **under_scores** in variable names?

This is a question programmers often discuss. The answer depends on who you ask:

### **Underscores:**


Many programmers prefer to use underscores (date_of_birth), especially in SQL databases.


Underscores are often used in PHP documentation.



### **PascalCase:**


PascalCase is often preferred by C programmers.


### **camelCase:**


camelCase is used by JavaScript itself, by jQuery, and other JavaScript libraries.


<br>

### **When comparing use === instead of ==**
***

This is important due to JavaScript being a dynamic language so using == might give you unexpected results due to it allowing the type to be different.

> **Wrong if (val == 2)**

> **Correct if (val === 2)**

Never use var use let instead


**Use const instead of let:**

This stops developers trying to changing things they shouldn't and really helps with readability.


Try and reduce nesting

An if within if can get messy and very hard to read, very quickly.


Use ternary operator instead of if for small statement.


**Use shortcuts for booleans:**


Try and avoid unneeded ternary statements:


Use lowercase file names:


MyFile.js should be **myFile.js**.

<br>

### **Template literals:**
***


> **Examples:**



    let firstName = "Mohammad";

    let lastName = "Jamal";
    
    let fatherName = "Mohammad Jamshed";
    
    let age = 26;
    
    let religion = "Islam";
    
    let email = "mohammadjamal876@gmail.com";
    
    let phoneNumber = 345698735678;
    
    let country = "Pakistan";
    
    let city = "Karachi";
    
    let maritalStatus = "Single";

    console.log(
        `${firstName} ${lastName} ${fatherName} ${age} ${religion} ${email} ${phoneNumber} 
         ${country} ${city} ${maritalStatus}`
    );


> **Output:**

Mohammad Jamal Mohammad Jamshed 26 Islam mohammadjamal876@gmail.com 345698735678 Pakistan Karachi Single







