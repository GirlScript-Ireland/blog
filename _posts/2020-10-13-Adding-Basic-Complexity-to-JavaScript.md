<div class="text-white bg-blue mb-2"><h1>Adding Little Complexity to JavaScript</h1></div><br>

<h2>Conditionals in JavaScript</h2><br>

So, talking about the conditionals, so conditionals are nothing but they let you execute a block of code depending upon a condition. You might be now thinking what’s a block or block of code. There are in total 3 conditional statements:<br>

```JavaScript
•	if(condition) {/*block of statements*/}<br>
•	else if(condition) {/*block of statements*/} <br>
•	else() {/*block of statements*/}<br>
```

There’s nothing much to do with that, to make you explain you the concept behind this takes a look below:

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js12.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js13.PNG)

So, the thing here is in the above example we have blocks of code that get executed or run depending upon a particular condition, as you can see when I reload my browser, what I see over the console is the output as shown. This happened so because let’s think of simple mathematics I have temperature = 30 assigned, now I ask you is a temperature greater than 20, yes that’s true so that false is actually stored here in a Boolean variable and hence you might decide to hangout that day as the weather is pretty much clear. So, temperature check was the condition here, Hangout is the processor block of code that was executed as a result if weather is fine. If the weather wasn’t clear you would have decided to stay in. Yeah that’s the point depending upon a condition check we execute a block of the statement; such statements are called conditional statements.
    
As you have seen above that not only single condition can be checked at a time, but more than one condition can also be checked using the Logical AND (&&) and Logical OR (||) operator.

So, now to some discussion about how we can use ‘let’ to declare variables and how is it different from ‘var’.  A variable declared using ‘let’ lets you declare a block-scoped local variable, optionally initializing it to a value. Now you might be thinking what is this scope thing. In a program, we have 2 scopes global and local. If something is global, let’s say “Sunrises from the east and sets in the west.”, that’s something that everyone knows but if I say “India is densely populated.”, then here we are talking about India only and no concern with the outside world. Similarly, let’s take an example to understand this.

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js14.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js15.PNG)

So, as in the example, we can see we have a variable declared using ‘let’ keyword in the outer scope whose value is 1 as we run the code we find an if() a conditional statement which checks if the condition (== is equal where = is assignment operator) x in global scope is 1 or not if yes, it creates a local x that exists as long as closing curly bracket for if statement appears and when it’s run the value of x within ‘if’ is 2 as we can see over console but outside viewing the x variable in the global scope, it’s still 2 hence we can say that using ‘let’ keyword we can create variable with the same name but the different scope of reach.

‘let’ allows you to declare variables that are limited to the scope of a <a link = "https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/statements/block">block</a> statement, or expression on which it is used, unlike the var keyword, which defines a variable globally, or locally to an entire function regardless of block scope. The other difference between var and let is that the latter is initialized to value only when a <a link="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let#Temporal_dead_zone">parser evaluates it (see link)</a>. Just like ‘const’, the let does not create properties of the window object when declared globally (in the top-most scope).

Variables are declared by let have their scope in the block for which they are defined, as well as in any contained sub-blocks. In this way, let work very much like var. The main difference is that the scope of a var variable is the entire enclosing function. We will further go though this topic once again when we discuss functions.

<h2>More about working with Conditionals</h2>

So, now let’s talk about the Ternary Operator. Ternary Operator is kind of alternative to if() and else() statements. The conditional (ternary) operator is the only JavaScript operator that takes three operands: a condition followed by a question mark (?), then an expression to execute if the condition is true followed by a colon (:), and finally the expression to execute if the condition is false. This operator is frequently used as a shortcut for the if statement.

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js18.PNG)

To Understand the use of a Ternary Operator and it’s used a replacement to the if-else statement, let’s understand a general example. Let’s say you go to the market to purchase a book if you are a permanent customer of that shop you are most probably going to get a discount, but if not then you have to possibly pay the original price. 

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js16.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js17.PNG)

<h2>Nested if-else</h2>
In some situations, we might need to check condition one after the other but not as a whole like if I pass the 1st condition than I check the second, otherwise I won’t go for that, this type of if-else methodology is called nested if-else. We will be demonstrating the same using the example below:

In this example we have considered a static example where we will be setting some variables like that refers like are you signed up for a webpage, if yes then are you verified, if yes are the payment credentials verified if everything goes right, you will have access to course.

In case you are signed up, but not verified it shows verify please and if you are not signed up, then you need to sign up.

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js19.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js20.PNG)

<h2>Switch Statements</h2>
Switch statements are another such alternative to if-else statements. In case the conditional statement looks for matching fall of case. The switch statement evaluates an expression, matching the expression’s value to a case clause, and executes statements associated with that case, as well as statements in cases that follow the matching the case.

To understand the use of the switch, let’s consider a particular example let’s say we have a website, the website has a different level of access properties for different sections. Let’s say the admin has the complete access, the blog writer has only content access and the viewer can just view the file.

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js21.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js22.PNG)

So, let’s break the code now as you can see here, we have a variable user storing a string data. Now in case of switch(matching_parameter) conditional statements, we have a parameter which we check matches the required condition or not. So, as soon as we enter switch, we test for different test cases and one which meets the required condition, the block of the statement contained within that case is executed.
The break statement forces the program flow to break and stop executing the other code as soon as the line is executed and that block is terminated there itself.
We could also have 

```JavaScript
	default: 
		//block of statement 
		break;
```

as the end to execute that particular set of statements if any of the conditions given doesn’t match with the parameter. If the break statement is not placed after every case what happens is that it considers all the falling cases below it as true and hence executes all of them, this is called Fall through.

<h2>Coercion and Falsy Values</h2>
The Variables have some kind of values associated with them generally, but if there’s nothing into them then also they contain something that just doesn’t make them a liability in the program.
So, variables that are just declared and are not assigned any value are undefined. Such variables when used as conditions for executing a block of the statement are generally taken to be false.

Similarly, we have 0, but 0 in actual makes sense that it’s an integer. In the same manner, we have ‘’ or “as empty strings that convey false when treated as Boolean in conditional statements. But in case of null, that’s pretty much different that even conveys false when treated as Boolean but here the change is that null is given to a variable when it’s expected that a variable always has a value associated to it or it will be undefined if it is being assigned something that doesn’t make any sense that’s null.

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js23.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js24.PNG)

Now let’s jump out to some crazy stuff, like what happens when we add a string to a number, how to compare the variables along with their datatype and values, and all stuff like that.

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js25.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js26.PNG)

== is only value check or comparison while === is value as well as type check at the same time. Hence that’s why 2==”2” is true but 2===”2” is false.

<b>Authour name:</b><i> Aman Kumar Dewangan(AkD)</i><br>
<b>Authour's Country: </b><i>India</i><br>
<b>Brief Experience History: </b><i>My name is Aman Kumar Dewangan, currently pursuing B.Tech in Electrical Engineering at National Institute of Technology Raipur. I am a proficient IoT Developer, Electronics Enthusiast, worked with no. of Micro-controllers including Arduino and Raspberry Pi. I am a Frontend Developer and beginner into Cloud Engineering as well. I have recently started working on Open-Source and generally program in C++. I have participated in many Hackathons as well.</i><br>
<b>Blog Content:</b> <i>The Blog is in Continuation to the previous blog on <a link="https://girlscript-ireland.github.io/blog/2020/10/12/Introduction-to-JavaScript.html">"Introduction to JavaScript"</a>, here we introduce you to the basics of conditional and switching statements.</i>
