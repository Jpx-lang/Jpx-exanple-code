# JPX Example Code

This page shows simple examples of JPX syntax including variables, functions, modules, loops, and error handling.

---

# Hello World

```jpx
Print "Hello World";
```

---

# Variables

JPX variables can be declared using `Global`.

```jpx
Global [name = "John"];
Global [age = 20];

Print "Name : $name";
Print "Age : $age";
```

---

# Arithmetic Operations

```jpx
Global [a = 10];
Global [b = 5];

Global [sum = a + b];
Global [sub = a - b];
Global [mul = a * b];
Global [div = a / b];

Print "Sum : $sum";
Print "Sub : $sub";
Print "Mul : $mul";
Print "Div : $div";
```

---

# Scanner Module (Input)

```jpx
[Scanner];

name = scanner.text("Enter your name : ");

Print "Hello $name";
```

---

# File System Module

```jpx
[Fs];

Fs.create.dir("myfolder");

code = "Hello JPX";

Fs.write("file.txt", code);
```

---

# Color Module

```jpx
[Color];

Print color.red + "Hello World";
Print color.green + "Success Message";
```

---

# Functions

```jpx
function greet(name) {
    Print "Hello $name";
}

greet("John");
```

---

# If / Else Statement

```jpx
Global [age = 18];

if (age >= 18) {
    Print "Access granted";
} else {
    Print "Access denied";
}
```

---

# While Loop

```jpx
Global [i = 0];

while (i < 5) {
    Print "Loop $i";
    i = i + 1;
}
```

---

# Error Handling

```jpx
try {
    Print "Running program";
} Catch (e) {
    Print "Error occurred";
}
```

---

# Full Example Script

```jpx
[Scanner];
[Color];

function greet(name) {
    Print color.green + "Hello $name";
}

username = scanner.text("Enter your name: ");

greet(username);
```

---

# Learn More

Visit the official repository:

https://github.com/jpx-lang
