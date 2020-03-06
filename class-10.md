#### Earthdate 06032020

# Error Handling and Debugging

Debugging is about deduction. It is a process of eliminating potential causes of an error to find the source. First, you must narrow the scope of the problem. The quickest way to acheive this is by examining the error report. The report will detail the type of error and the file and line on which the error was identified. Unfortunately, this isn't a needle straight to the error, because it is merely where the system dectected that something was amiss, and the error could be many lines before it depending on the nature of the code.

Begin addressing the situation by writing **console.log()** to identify values and objects that you are unsure of. And use breakpoints where things seem to be going awry. Especially in a group setting, seek the advice of other programmers--try describing what should be happening and where the complications seem to be arising. Browser developer tools are immensely helpful in this process. 
You can also use **console.info()**, **console.warn()**, and **console.error()** to inspect your code. And **console.group()** allows you to submit a group of messages to the console. In browsers that support it, you can also use the **console.table()** method to output objects or arrays that contain other arrays or objects. And with the **console.assert()** method, you can test if a condition is met, and write to the console only if the expression evaluates to false.

You can create a breakpoint in your code using just the **debugger** keyword. It will automatically create a breakpoint when the dev tools are open. However, you can also place the debugger keyword within a conditional statement so that it only triggers if the condition is met.

**WARNING: Make sure you remove error handling code from the final product!**

Also available for your error-correcting pleasure is the **Try / catch / finally** methodology. First, you specifiy the code that you think might throw an excepton in the *try* block. If the *try* code block throws an exception, *catch* steps in with an alternative set of code. The contents of the *finally* code block will run either way - whether the *try* block succeeded or failed. It even runs if a return keyword is used in the *try* or *catch* block.

Once you think you have identified the area of concern, inspect the code more closely. If you have set breakpoints, you can inspect variables around the area to see that they contain the values you would expect. Use the console here. break out pieces of code and test them in the console with your own variables. Check the number of parameters in a function, or the number of items in an array. And don't get discouraged. Complicated code may take several takes to identify missteps.
