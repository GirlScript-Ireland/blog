<h1>Introduction to JavaScript</h1>

Welcome to Complete JavaScript Guide, A that starts from basic like DOM Structure, declaring variables, learning about functions, declarations, classes most modern things like promises async JavaScript, spread operators, and most importantly DOM manipulation and building projects with it. Throughout the course, we will try turning out the toughest topics in the easiest possible way, so that programming becomes fun and engaging. We will wrap up all the concepts related to JavaScript in these modules

JavaScript is a full-fledged dynamic programming language that can add interactivity to a website. It was invented by Brendan Eich (co-founder of the Mozilla project), the Mozilla Foundation, and the Mozilla Corporation. JavaScript is versatile and beginner-friendly. With more experience, you'll be able to create games, animated 2D and 3D graphics, comprehensive database-driven apps, and much more. JavaScript itself is relatively compact, yet very flexible. Developers have written a variety of tools on top of the core JavaScript language, unlocking a vast amount of functionality with minimum effort.

JavaScript has developed a lot and hence there’s a need for the guide which is not a band-aid guide over the existing ones but a completely full-furnished fresh guide, that teaches you a lot about JavaScript, directly by writing the code as well as by understanding some of the behind the scene concepts of JavaScript. How it works??, How the Global Execution context works? How ‘this’ keyword works?? How the spread operator and rest operator are different from each other and a lot more topics like that.
Learning all these Topics about JavaScript is necessary, it’s important but what’s more important is learning with fun, a content that is engaging that you enjoy the whole lot learning process and that’s why we have included projects to give more emphasis on project-based learning. The projects are DOM based so that the process of learning doesn’t seem boring and practice and we learn where to implement JavaScript.

So, we will initially start with installing the tools and writing our very first code. We will do the #classic “Hello World!!” and after that, we will move on understanding about variables, conditionals, and loops, though the guide is not structured in a bookish manner. We have modified the guide structure to make it more fun-learning and we can understand every topic int the easiest manner. So, the guide structure is a bit different and we have included challenges as well to get the best out of it so that you can get to know you have got the concept or not like we have learned it here and I am implementing it here.

Pre-requisites: Zero (0) Seriously, you can begin with no knowledge. You don’t need to have any prior knowledge of other languages like C, C++, Python, Java, etc anything like that you can directly learn it as a very first Language. (Warning: HTML and CSS are not Programming Languages 😊) And we hope it would be whole lot fun learning JavaScript.
Just 10 minutes of daily walk through each module, you can be a JavaScript expert. There will be a whole lot of knowledge of insight behind the scenes of JavaScript that you are goanna thoroughly enjoy. One request from our side if you find anyone stuck at any point just guides them here to this guide and if you find it helpful then do share it with your geeky programmers’ community and friends.

Though we have tried to cover almost everything as a programmer it’s your responsibility as well to keep looking on to the original documentation of these languages over the internet for better knowledge.

Link: https://developer.mozilla.org/en-US/docs/Web/JavaScript

<h2>What are JavaScript Engines??</h2>
  
Actually, before writing code in JavaScript, you need to know where we are gonna write and run our code and probably, you might be excited about that, so hold on for a moment first let’s move through the software needs first. 

So, for writing the code we will be using VS Code (Visual Studio Code), which is the favorite of most people and gaining a whole lot of popularity. There are a lot of themes and plugins that we can install. Though you can also use codepen.io (Brackets.io – offline version) or sublime for the same purpose no issues.

So, let’s start now:
1.	So, create a folder probably with name ‘Js’ and within it create another folder name ‘hello’, feel free to name it however you like.
2.	Fire up (Open) the VS (Visual Studio) Code.
3.	Drag and drop the ‘hello’ folder over VS Code if you are still following what’s mentioned.
4.	Now the classic way since the ages that have been continuously followed is creating the 2 files namely:
5. 	Within index.html write the following code:

(1) index.html (2) script.js 


```HTML
   <!doctype html>
   <html lang=’en’>
   <head>
	  <meta charset=”UTF-8”>
	  <title>Document</title>
   </head>
   <body>
   Some content is to be added here, wait hold on.
   </body>
   </html>
```
6. It's completely Ok to have the script.js file empty
7. Now add these two lines in betwwen the opening and closing tags of the body.	

```HTML
   <script src = ”script.js”></script>
   <h1> Hello World</h1>
```
8. Go to the file and Open it with Web Browser and you will see Hello World written in big headings over there, but there’s nothing to do with Js as the script.js file is empty.
9. Now right click on the browser screen of page, a drop-down menu select ‘Inspect’/’Inspect element’ and go to console option than.

![Alt](https://github.com/amandewatnitrr/blog/blob/master/_posts/Js_Tutorial_Images/js2.PNG)

10. Now once you are done with this part, go to script.js over VS Code.
11. In the script.js in VS Code write the following line as shown and save it:

```JavaScript
console.log("Hello JavaScript");
```
13. As soon as you save it and reload the page by clicking on the reload button, over the console we see “Hello JavaScript” written over there. This is the proof we can load up our JavaScript in the HTML file.
14. This brings us to a very important question,” Is it the right way to run the JavaScript Code??”

Yeah! It’s fine, all clear 100% there’s no problem with it. But this is not the only way to run the JavaScript and we need to know why this is all happening and how can I run the same code in a bit advanced manner??

![Alt](https://github.com/amandewatnitrr/blog/blob/master/_posts/Js_Tutorial_Images/js2.PNG)

So First of all, we need to understand JavaScript is just like other languages like C++, Java, or Python. It needs a certain thing, tool or set of software so that this JavaScript language can be converted into Machine-Level Language and that’s the most foundation of running the JavaScript and since the very history long we have always seen that the JavaScript comes with a compiler that converts JS code into executable code. Nobody bothers that there’s a compiler running our code. The fact is this engine was already having compilers and people think that they can be run only over browsers. Some of the JavaScript Engines namely are ‘V8’ and ‘Spider Monkey’.
