# Reflections

One of the core competencies of a programmer! This stuff is equal parts infuriating and satisfying. It's like being a detective in the most boring and low stakes crime drama on TV.

## Reading

[What Went Wrong? Troubleshooting JavaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_went_wrong)

1. Name some key differences between a Syntax Error and a Logic Error.

    Syntax errors are spelling errors that cause the program to not run at all or stop working partway through. Logic errors are more sneaky and insidious because it's garbage in, garbage out.

2. List a few types of errors that you have encountered in past lab assignments and explain how you were able to correct them.

    Where to begin...

    - Using Math.round combined with the PROJECTED_SALES_CURVE from the salmon cookies assignment caused an edge case error where values of 1 for min and max customers and 1 for avg cookies rounded down to 0 cookies sold in the hour, which was unintended logical behavior.
    - Using the constraint validation API caused all sorts of issues because the submit event fires last after validation checking, so that if you use `.setCustomValidity` it will set it and never update it for a function called form within the submit callback function.
    - Tons of typing errors where JS handles number input as strings in the form, and it desperately needs to be converted in the code.

3. How will this topic continue to influence your long term goals?

    I will continue to mess up and hope to run into all sorts of errors to deepen my ability to pull a rabbit out of a hat when I see something stupid, because I'll have run into it in the past.

[The JavaScript Debugger](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_are_browser_developer_tools#the_javascript_debugger)

1. How would you describe the JavaScript Debugger tool and how it works to someone just starting out in software development?

    Debuggers are an incredibly useful concept for any programming language. They allow you to pause the execution of your code, see the state of variables and functions at any point, slowly circle on when and why a code stops working, and more. It is the CSI lab for finding out who did the crime.

2. Define what a breakpoint is.

    A breakpoint is a pause button that you can place on any line in your code. You can step over them, step into them (in the case of breaks at function calls), and step out of them.

3. What is the call stack?

    - When you call a function, the system sets aside space in memory for that function to do its necessary work
    - We frequently call such chunks of memory **stack frames** or **function frames**.
    - More than one function's stack frame may exist in memory at a given time. Only one is **active** at a time.
    - These frames are arranged in a stack. The frame for the most-recently called function is the active frame.
    - When a new function is called, a new frame is **pushed** onto the top of the stack and becomes the active frame.
    - When a function finishes its work, its frame is **popped** off of the stack, and the frame immediately below it becomes the new, active, function on top of the stack. This function picks up immediately where it left off.

## Things I want to know more about

1. Is there a way to split the dev tools into a new browser window for a separate window, or some other way to make it more manageable to root around in the many nested windows and sections?
