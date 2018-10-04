# eggplant 🍆

A stack-oriented interpretted language created using Felix Plesoianu's "Make Your Own Programming Language" (http://scratch-lang.notimetoplay.org/index.html).

🍆 is written entirely with emojis.

## Printing
* 📠 (**Print**) pops the item on top of the stack and prints it
  * e.g. `5️⃣6️⃣ 📠` pushes 56 to the stack and then pops and prints it, leaving the stack empty. Note the space between the two elements.
* 📠📑 (**Stack Print**) prints whole stack (stack remains intact)
  * e.g. `5️⃣ 6️⃣ 📠📑` pushes 5 and 6 to the stack and then prints `5️⃣ 6️⃣`. Note, again, where spaces are placed.

## Math
* ➕ (**Addition**) pops the two items on top of the stack, adds them and pushes the result to the stack.
* ➖ (**Subtraction**) pops the two items on top of the stack, subtracts them and pushes the result to the stack.
* ✖️ (**Multiplication**) pops the two items on top of the stack, multiplies them and pushes the result to the stack.
* ➗ (**Division**) pops the two items on top of the stack, divides one by the other and pushes the result to the stack.
* ✔️ (**Square Root**) pops the item on top of the stack and pushes back its square root.
* ❇️ (**Mod**) pops the two items on top of the stack and pushes back its modulo.
* 0️⃣1️⃣2️⃣3️⃣4️⃣5️⃣6️⃣7️⃣8️⃣9️⃣ (**Digits**) pushes given number to the stack

## Stack Operations
* 🔂📑 (**Top Duplicate**) duplicates top item on the stack
* 📤📑 (**Pop**) discards top of stack
* 🔀📑 (**Swap**) swaps top of stack with second item on stack
* 🔂🔂📑 (**Second Push**) copies second item on stack and places copy on top of stack
* ⏫📑 (**Third Push**) brings third item on stack to top

## Variables, Constants, Strings
* 🍆`<variable>` (**Dim**) defines a variable named `<variable>` (`<variable>` is expected to be an emoji)
  * e.g. `🍆😊` defines a variable named `😊`
* 🛄🍆`<variable>` (**Store**) pops topmost value on the stack into `<variable>`
* 🛅🍆`<variable>`(**Get**) gets value of `<variable>` and pushes it to the stack
* 🐘🍆 (**Constant**) defines a constant and pushes it to the stack
* `✏️` (**String**) declares a string and pushes it to the stack
  * e.g. `✏️ hello world✏️`

## Functions
* ♻️ (**Function**) function declarator (must be followed by an emoji to name the function)
* 🚫 (**End Function Block**) function block end
* e.g.:
  * `♻️ 🍉 
      ✏️ 🌍✏️ ✏️ 📠 
    🚫`
  * defines a function 🍉, which prints the string `🌍`
  
## Arrays
* 🌜 (**Array Declarator**) defines the start of an array
* 🌛 (**Array Closer**) defines the end of an array
* 📏 (**Array Length**) pushes length of array to the stack
* 📬 (**Array Subindex**) references item in array
