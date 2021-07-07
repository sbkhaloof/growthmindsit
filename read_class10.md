# In memory storage
## Understanding the JavaScript Call Stack
1- What is a ‘call’?
##### At the most basic level, a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).
2- How many ‘calls’ can happen at once?
##### Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.
3- What does LIFO mean?
##### When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.
4- Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
![](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d3/Call_stack_layout.svg/342px-Call_stack_layout.svg.png)
5- What causes a Stack Overflow?
##### A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.
## JavaScript error messages
1- What is a ‘refrence error’?
##### This is as simple as when you try to use a variable that is not yet declared you get this type os errors.This is also a common thing when using const and let, they are hoisted like var and function but there is a time between the hoisting and being declared so when you try to access them a reference error occurs, the fact that this happens to let and const is called Temporal Dead Zone (TDZ).
2- What is a ‘syntax error’?
#####  this occurs when you have something that cannot be parsed in terms of syntax,
3- What is a ‘range error’?
##### Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up
4- What is a ‘tyep error’?
##### Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.
5- What is a breakpoint?
##### The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.You can also add conditional breakpoints by right-clicking a previous set breakpoint, which will make your program stop at that point only if a condition is met, this is awesome for when you want to debug huge cycles for specific values. 
6- What does the word ‘debugger’ do in your code?
##### A debugger is a tool that is typically used to allow the user to view the execution state and data of another application as it is running. Debuggers allow users to halt the execution of the program, examine the values of variables, step execution of the program line by line, and set breakpoints on lines or specific functions that, when hit, will halt execution of the program at that spot. In this view, seeing how the program is viewed by their computer, the user can discover how a program flows, identify incorrect code and data, and find semantic errors in the program.