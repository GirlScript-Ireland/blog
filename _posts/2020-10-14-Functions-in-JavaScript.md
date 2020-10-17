<div class="text-white bg-blue mb-2"><h1>Functions and Scope in JavaScript</h1></div><br>
<h2>Functions in JavaScript</h2><br>

A function is a named block of code that can be invoked from other parts of the program. Due to Functions being one of the most foundational topics in JavaScript many things weren’t being discussed in deep yet. JavaScript is functional programming you can say. Now a thought might strike out why are we using these functions, what’s the benefit.<br><br>The idea behind the function is to put some commonly or repeatedly done tasks together and make a function so that instead of writing the same code again and again and making desired changes every time where ever we require it and for different inputs we can call that function.<br><br>JavaScript has built-in as well as user-defined functions as well. Like console.log () it’s an inbuilt function in JavaScript, similarly, user can also create their functions. We can create functions in JavaScript using the keyword ‘function’.
<br><br>So, let’s start up on this with some examples:

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js27.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js28.PNG)

So, as seeing the above function, a function as it’s a declaration and the other when it’s called. Just defining a function can’t make it automatically executed, we need to call wherever we need to execute it.<br><br>
<h2>PASSING VALUE/VARIABLE TO A FUNCTION</h2><br>

So, eventually, if we define a function, it’s the value of an expression based on certain no. of inputs. Similarly, here in JavaScript we will be passing variables here and show what all we can do with that.

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js29.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js30.PNG)

So, in the example mentioned above, I declared a function named display() that takes 2 inputs your name and your age and prints it in a given format. A function can be with/without arguments. As we can see the function minimizes the need for writing the same code and changing it back again and again rather give just different inputs and produce output in the same manner again and again the way we want.

<h2>RETURNING VALUES FROM A FUNCTION</h2>

As we have seen till now, how we can minimize the task of writing code, again and again, using a function, let’s now move onto how we can return some value from a function.
Returning some value in the sense means giving some kind of data back as output. Let’s consider the following example for this purpose.


![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js31.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js32.PNG)

So, let’s again break down the code and understand what’s going on. Basically, I have a function declaration with name display as the previous case, the function takes 2 arguments as input from the user and then stores the new string generated after processing in a variable and return that variable as an output. The string stored in that variable is stored in a variable declared in the execution-able scope and the output is printed on the console.

<h2>Understand the context in JavaScript</h2>
Many of the programmers out there say that JavaScript is odd, people say it’s weird, but no that’s not the point it’s actually about understanding the context of JavaScript that many don’t.
So, let’s first do something a bit crazy. Let’s see this example:


![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js33.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js34.PNG)

Now, I don’t know if you realized whether that the function calling code before the function has been declared, it’s like I used a time-machine to go back into the past in time before I was born and tell, hey you know me. But something similar happens in JavaScript. So, does this statement makes sense, yeah and it even works. So, this is all about the global context of the JavaScript and to understand how this global context works. JavaScript has a bigger context in which everything resides.
The global context differs a bit when we execute the code in the browser and Node.js, let’s consider the below piece of code as an example:

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js35.PNG)

So, it’s completely clear that above script.js file runs fine and then I moved to the console and did the same thing back but this time I used ‘window.name’ instead of name and rest, everything’s the same, and it worked pretty well the same way.<br>
So, there’s just a bit different with the global context if you run it over the Node.js, here it might show ‘window’ is not defined because there the global context will be run by node.js, and hence the global context is not available there. The global context differs when we execute it in code and the one we do in the browser. There’s always a context there with the JavaScript Engine and that context is responsible that all of the things are registered inside the context, so that once the function is been registered then that function is wrapped up and put inside a global context. Whenever we need to do that when the code executes it is aware of those functions, that’s the reason why even using the calling code of function before the function declaration works fine.

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js36.PNG)

<h2>Code Hoisting in JavaScript</h2>
Understanding Context makes it clear for you to understand JavaScript in simplified and you will never consider JavaScript as a weird language again. So, in the previous article, we were mostly talking about the global context and now we will discuss the variety of context in JavaScript. So, now we will be discussing the working of Context I	n JavaScript. Whenever we say there’s a context available to us just remember there are 2 types of major context available to us:
1>	Global
2>	The One that’s being executed right now, if you are running a script file.
Let’s learn this topic with an example:
The whole idea of Global context is to majorly collect the information but as soon as we want to run some code like console.log(). To make it run completely the execution context will come into picture which will be responsible for running this function. The window object is majorly tied with the browser. 
Execution Object brings a whole lot of new things into the picture:
1.	Variable Object
2.	Scope Chain
3.	This
Concerning execution context we have to follow 2 rules:
1.	Function declarations are scanned and made available.
2.	Variable Declarations are scanned and made undefined.
So, let’s catch up with little examples:

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js37.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js38.PNG)

It’s pretty much clear from the above example, how the global execution context works and how it follows the 1st rule of the execution context. Now let’s bring some crazy stuff into this as we are now ready to have some test and try. For that let’s turn the tip into the string and check what happens😋.

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js39.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js40.PNG)

It’s pretty much clear from the code what’s happening, what if we still want to pass a string but treat it as a number, we have a function ‘parseInt(variable_name) dedicated for that. Let’s check out the next code block and implement it.

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js41.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js42.PNG)

Now let’s move to another similar example, but this time we are going to declare the function in another way, so let’s check out our code.

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js43.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js44.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js45.PNG)

On running we will get to know that giveTip is a function but givebigTip is a variable but not a function in actual and this gives an error, so there is variable inline 13 that we are trying to use in actual and is undefined and that makes pretty much sense. The Global Context doesn't know about it. They are functions but treated like ordinary variables and that is why code hoisting comes into the picture.
So if the code is right what can probably go wrong, if you are thinking it that way you are right as it is a variable, we will need to declare it first and then use that variable so the correct set of code that would work fine must be like this.
This is how it works. This is the difference in calling a function and a function variable in JavaScript. This is a part of simple code hoisting.
Now we must also talk about the 2nd rule of the global execution context, that the variable with nothing initialized must be ‘undefined’, but I guess we should check, because there’s a lot of surprise waiting in there for you.
This must produce two different outputs like line 1 will show undefined and the 2nd one will show me “Aman” that is the statement 1 knows about the existence of variable declared inline 2 but just isn’t aware of the value in it, hence it shows undefined.


![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js48.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js47.PNG)

So, This is getting pretty much long and weird but I want the readers, to get complete clarity of the topics, so one more point that must have been included in case of local and global context is that the relation between global context and execution context is just like a Last In First Out Stack(LIFO), that is the plate which is at the top needs to be displaced to take out the plate below it, and that sounds quite logical and obvious. So, look at the following example and hope that will be clear to you.

So, as we can see the line 1 recognizes the existence of name variable but has nothing stored hence shows blank which means undefined, as the name variable now gets initialized when we call the showname() function it’s local scope has a different value for that variable that’s ‘akd’, it says for whatever name of him you might be knowing I don’t care I know him as ‘akd’, as soon as the local scope of the function ends we then again try printing the value of the variable in the global scope and that’s the same thing that we expect as initialized or in simple term by which name people globally know him as ‘Aman’.

<h2>Scope Chaining in JavaScript</h2>

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/Scope_Chaining.PNG)

As of now we have thoroughly discussed the Variable Object and the context now it’s time to discuss the Scope Chain, so for this, we will be discussing a short scenario. Let’s say we have 3 businessmen with the name Blue, Orange, and Green. Let’s say Blue is richer than Orange, and Orange is richer than Green. So Green can ask for money from Orange as well as Blue if he needs it, but Orange can ask only money from Blue as Green is less rich compared to Orange so why Orange would ask money from a guy who has even less money than him. Blue being richest among all can’t ask both of them for money as he is the richest among all, though Orange and Green are free to ask him for money as Blue is much richer.
So, I guess you might have understood the scenario and able to visualize the things if I talk in Mathematical terms the Green covers the region of Both Orange and Blue, Orange covers the area of Blue and Blue is the complete circle in itself, with other circles lysing inside it.

So, now let’s try visualizing it through some code.


![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js49.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js50.PNG)

What we did here is let’s say the global scope of the program to have the name Blue which has 10,000$, now there’s another businessman under blue named Orange(basically referring to the function) who has no money of his own so he asks it from the blue, blue gives his complete money to orange for business, that’s what we can visualize out of this code in the easiest possible way. So that’s why line 2 prints the value of an amt variable in the global scope, but as orange has no money or separate amt variable of his own, it automatically gets referred to the global variable.
Now let’s make a change into the program or the scenario over here. Let’s say initially the orange guy has some money of his own let’s say 5000 i.e. it has its own variable ‘amt’, in that case, it will not refer to the global amt but will run his business with the amount he already has. Let’s understand the same through code.


![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js51.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js52.PNG)

So, trying to understand and relate the scenario we can say why to ask for money if I can use my own money for the business, that’s why the log command refers to the amt variable within the function and not the one in the global scope.
The reason why people JavaScript a weird language is because it’s really weird, for example, if you are asked about how you identify any scope, and the answer most probably is anything within curly braces that’s right but in JavaScript, it’s not truly considered as a scope. Though it is a scope, don’t get wrong there but it’s not truly scope in the world of JavaScript but rather an only element that is tied to a function, but not in a case like for, if, else, switch, etc.
Now let’s bring the third businessmen into the picture here.

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js53.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js54.PNG)

Now, have a look at this code so now we can visualize it as 3 businessmen sub-local under local under global. The Global Leader has 10,000$, the person working under him that is the local guy has 5000$ but the sub-local guy working under him has no money of his own so he asks to his superior the local/orange guy for the money and he gives it and Remembers the Richer person cannot ask money from the poor guy.
Now, what if I also give some money to the green guy as well, yeah you are not getting it once the green guy also has his own money, he won’t ask the blue or the orange guy for the money. In that scenario, the code would be somewhat like.

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js55.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js56.PNG)

So, now as the green function has it’s own ‘amt’ variable it won’t approach the block superior to it for the value.

<h2>What is this “This” in JavaScript??</h2>
Many of you who have programmer friends, who might be familiar with JavaScript might already be telling you about JavaScript and the weirdness of the language and especially about this ‘this’ thing. For now, this would be just an introduction to this topic, and once we learn other things and find our-self capable to understand the deep concept we will bring them to light again.
So, to understand this let’s start with what is this ‘this’ in actual, sounds crazy but yeah!!
Enter the following code in your JavaScript Engine and see what’s the output
console.log(this);
Most expectedly you are going to get different outputs on different engines because every engine has its global context, but most people prefer node.js or the browser only. So, there are 2 possible outputs as of being only concerned with node.js and browser:

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js57.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js58.PNG)

The first one is the empty set i.e. for node.js engine just without anything else in a .js file refers to an empty scope/set. While the same thing over browser refers to a window object. 
Now let's try to experiment and visualize things by doing some basic things like declaring variables and functions. So let’s do something with the code:

![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js60.PNG)
![Alt]({{site.baseurl}}/assets/Js_Tutorial_Images/js59.PNG)

So, it’s quite confusing to understand and things appear like it doesn’t make any sense so, for now, let’s keep a hold on to this topic, not to confuse much to our readers, for now, let's keep it clear cut that the code gives us access to the global object window. When we have much better knowledge about syntax and other concepts we will move back onto this topic and then we will understand it in much more detail.

<b>Authour name:</b><i> Aman Kumar Dewangan(AkD)</i><br>
<b>Authour's Country: </b><i>India</i><br>
<b>Brief Experience History: </b><i>My name is Aman Kumar Dewangan, currently pursuing B.Tech in Electrical Engineering at National Institute of Technology Raipur. I am a proficient IoT Developer, Electronics Enthusiast, worked with no. of Micro-controllers including Arduino and Raspberry Pi. I am a Frontend Developer and beginner into Cloud Engineering as well. I have recently started working on Open-Source and generally program in C++. I have participated in many Hackathons as well.</i><br>
<b>
<b>Blog Content:</b> <i>The Blog is in Continuation to the previous blog on <a link="https://girlscript-ireland.github.io/blog/2020/10/13/Adding-Basic-Complexity-to-JavaScript.html">"Adding Basic Complexity To Javascript"</a>, here we introduce you to the functions in JavaScript and Scope Chaining in JavaScript.</i>
