When this code is run in Node, e.g. node index.js, what are the two stages of execution for this file called, and which order do they happen in?
Answer: The two stages of execution for this file are bar() and baz().  bar() is called first, then baz() is called.

Write an explanation, using as much space as you need, relating to how the first stage of execution for this file operates. 
For example, identify the high level steps in a line by line overview and then define what each of those steps are accomplshing.
Answer: the first state of execution occurs when bar(); is called at the bottom of the page. First the compiler there is a variable called foo and then foo is assigned the value of 'bar. 2nd, a bar() function is found and within that bar() function the variable foo is assigned the value of 'baz'. 3rd, a baz() function is found and it is accepting/looking for the parameter 'foo', also, within the baz() function the foo variable is assigned the value of 'bam' and the bam variable is assigned the value of 'yay'.   4th  baz() function is called which returns 'bar'.  5th bar() function is called, 'foo' and then 'bam' are displayed.  6th baz() function is called.

Write an explanation, using as much space as you need, relating to how the second stage of execution for this file operates.
For example, identify the high level steps in a line by line overview and then define what each of those steps are accomplishing.
ANSWER: baz() function is called, which is looking for the foo parameter, the foo parameter is assigned the value of 'bam' within the baz() function.

During the second stage of execution how many scopes have been registered by the engine?
ANSWER: 2 scopes have been registered by the engine during the second stage.

Which segments of the code do they belong to?
ANSWER: one scope belongs to the function baz(foo) function, the other scope is within the function bar() function.

Please identify any variables/refs and which scope each belongs to?
ANSWER: The variable foo = 'baz' is within the scope of function bar().  the variable foo = 'bam' and bam = 'yay' are within the scope of function baz(foo) function.

When line 13 invokes the baz function, which foo will be assigned a value of bam? More specifically, bam will be assigned to the foo in ??? scope. Give a brief description in your own words to support your conclusion.
ANSWER: the baz function will be assigned the value 'bam' and is within the function baz(foo) scope.  This is because when baz() is called, it looks for the value foo and finds that foo = 'bam'.

Which scope, if any, will the variable bam on line 11 be registered to when the first stage of execution occurs on this file? Provide a brief description in your own words to support your conclusion.
ANSWER: function baz(foo) will run when the stage of execution occurs on line 11 and 'yay' will be the value assigned to it, however, bam is not a function, so the 'yay' value will remain behind the scenes only.

For each line, 16 through 19, what is the return value for each?
ANSWER: 16 -- returns 'baz'    17 -- returns 'bar'  18 -- returns 'yay'  19 -- returns 'bam'