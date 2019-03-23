# JavaScript assignment

## Some useful resources
* Some [JavaScript tutorials](https://www.htmldog.com/guides/javascript/)
* The complicated [resources in the You Don't Know JS](https://github.com/getify/You-Dont-Know-JS) series, including [your reading last week](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch2.md)
* [A resource for CSS/style/colors](https://htmlcolorcodes.com/)  
* [An excerpt from a specific workshop site](https://witny-summer-guild-2018.github.io/day_4_exercise_2.html) (for a different audience than yourselves) which addresses some common questions about jQuery
* [The simple JSFiddle example from class](https://jsfiddle.net/2of65j8q/)
* A [W3Schools resource on JavaScript output](https://www.w3schools.com/js/js_output.asp)
* Google, Piazza, your classmates, office hours, lab time!

## Included files
* This `README.md`, which you should edit with answers to the questions
* `jsPracticeLab.html`, which you'll need to edit and try out
* `jquerylib_submit_example.html`, which you'll need to edit and try out

## Your goals for this lab

### Broadly
The aim for this lab is to practice adapting to and understanding code in a new-to-you (or not) language and its own libraries/packages -- JavaScript, in this case.

The programming skills you have built up till now are useful for *Python programming*, but, more than that, they extend to fundamentals of many kinds of programming.

This experience is *not in any way* about becoming an expert JavaScript programmer. Instead, it is about using what you *do* have experience with -- and your skills in *learning new things* that relate to programming -- in order to make educated judgments about some brand new-to-you code, even if you haven't learned in detail about it yet. That's part of what being in technology -- or even technology-adjacent -- will often mean.

### Specifically

Below are a bunch of questions and indications of things to do. For each indication of something to do with code, there is also an accompanying question to answer or brief explanation to give.

**To complete and submit this assignment, you should:**

* Fork (and clone) this repository
* Add our instructional team as a collaborator to your fork (see instructions for adding collaborators on Canvas)
* Edit this `README.md` file with answers to the questions/prompts, briefly, using Markdown formatting so that the questions appear in bulletpoints and the answers appear clearly below each respective question, *not* as bulletpoints.
* Add all names of those who worked on this (as indicated below)
* Make the changes that are indicated below to each of the `.html` files with JavaScript programs provided. (You'll probably do this concurrently with answering questions)
* Commit (as you go) and push your changes to all three files to your GitHub forked repository.
* Submit a link to your repository on Canvas. (This HW doesn't have an autograder -- it will be graded by hand/by humans this time.)

### Important notes
* You are *more than* welcome to work together on this, but **you must <u>each</u> submit a repo to be graded on it**, so if you do work together, you should do the following:
	* Make sure each one of you understands all the work -- YOU are responsible for using and knowing this information
	* Write each person's name & uniqname who worked on the assignment together on your submitted `README.md` file (you'll see a space for this below)

* In answering questions, please make sure the formatting is clear to read and that you have updated the names of everyone who worked with you, with your name first (see below).

* In answering questions, assume all of the questions include a *explain briefly* note -- you do NOT have to, and should not, write extended paragraphs. Be as concise as you can and explain in your own words. Don't worry about "whether it's enough" -- just worry about conveying your understanding so you can read it later, or even give it to someone else, and the answers will help/make sense.

* It is not acceptable to copy and paste answers from the internet and submit them as your own. If you cite things, make sure you provide a citation, including to links. If you get information from a resource and rephrase it so you're basically explaining an idea, that's just fine for an explanatory purpose in this assignment, but you *must* cite any quotes or examples that aren't yours.

* **For grading:** we are grading on...
	* Following the instructions
	* Approximate correctness of the code edits
	* Careful & clear answers to the questions
	* Correct answers to the questions
	* Slightly more than half the 1000 points will come from answering the questions. The rest will come from your edits to the code.

### Names of people you have worked with on this assignment
* **Heather Shoecraft (hnhampt)**
* Monica Comeau Pagani (mpagani)
* Sabah Habib Pirani (sabahp)

## Questions & code instructions

### The first questions address the `jsPracticeLab.html` file.

* **This is just an example question.**

This is what an example answer should look like. If you want to include some code, which you probably don't have to do, you can, like this:

```js
Some JavaScript code
```

* **What does a code comment look like in JavaScript? What character/s do you have to put before a comment?**
A code comment is greyed out, same as a comment in Python, but they are preceded by // (instead of #).

* **Explain what needs to happen to get a JavaScript program to "run", given the JavaScript you've seen in this assignment.**
To "run" a JavaScript program you open it using a web browser.

* **What functions in JavaScript seem to be similar in function to the `print` function in Python? (There are two.) Why might you use one and not the other? Explain briefly.**
alert - This generates a pop up message
console.log - This makes a comment in the console, which is accessed by Inspect Element then switching to Console (using Firefox). This is similar to using print statements in Flask--they aren't visible in the web browser, but are visible in bash.

I would use alert if I wanted the average/"normal" user to read the message and console.log if there was something I needed to communicate to other programmers or developers.

* **What code would have to comment out to get rid of the pop-up box when you load the page? (Related to the last question.) Do that in the code file, and then, add code so that a text box will appear that contains the current date and time! *HINT:* Look through the rest of the code first...**
To get ride of the pop up box, comment out line 12
```js
alert("hello")
```

I added the following on line 13 (and also learned that spaces are okay (new Date)).
```js
alert(new Date());
```

* **How can you put your own name at the top where it currently says "A name"? Explain very briefly how to do so, and replace `A name` in the web page with your own name.**
In the displayInformation function change the h1 (header) line from "A name" to "Heather Shoecraft" (line 17).

* **What does the word `document` represent in this code? Explain briefly.**
I believe document represents the page that is viewed in the web browser. It seems similar to creating classes with self.xyz, where document.xyz has specific parts to it which, as a whole, are one document.

* **What is happening in line 12 (
		`document.querySelector('#items').innerHTML = document.getElementsByTagName('li').length`
)? Explain, briefly (<= 2 sentences).**
```js
document.querySelector('#items').innerHTML = document.getElementsByTagName('li').length
```

The first half of this statement is setting up the variable name that will be used in the CSS.
The second half is getting the value: find the elements with the tag 'li' then get the length of that query. Similar to Python len(), but .length goes at the end.

* **What color would the background of this page be <u>if there were no JavaScript in this page</u>?**
It would be white (which appears to be the default). The style of the body is modified to be neon green in the JavaScript section of the code (line 22) and is not defined at all in the style section.

* **Why are there a couple of gray boxes on the screen with a different colored border? How could you edit this code to make them a different color? Explain briefly. Then edit the code to make those boxes some shade of blue, of your choosing.**
The javascript modifies the body of the document to green, but the grey boxes appear because they are tagged <p> which has a different style defined.

* **Edit the code so that, if you highlight `McGill University` and copy it, you see the text `O Canada` near the bottom of the page. Briefly explain why you made the edits that you did -- how did you know/figure out what to do?**
I used a lot of trial and error to figure this out. My goal was to model it after the hightlight/copy code for University of Michigan. First I needed to write a function that would be executed when McGill University was copied. The function is defined on lines 32-34.

Next, I needed to modify the list so that when the copy action took place, the function would be called. See line 74.

Finally I duplicated line 78 and modified it to the below statement.
```js
	<div id="canada">
```
Something didn't seem to be working quite right as Go blue! was appearing below my Wow and Equinox buttons, but O Canada was appearing before them. Then I realized that after each <div> I needed </div> (there was currently only one in my code). Fixed that and now both messages appear above the buttons.

* **In the original code, when you click the button that says `Wow`, you see a text box! Wow. Explain briefly in your own words why the following code causes that to happen:**

```js
function handleClick(){
	alert("hello");
}
```
**and**

```js
<button onclick=handleClick() id="wow-button">Wow</button>
```
The first part of this code defines a function called handleClick. When the function is called an alert (pop up window) with the text "hello" will appear.

The second part of this code is saying when the button called "Wow" is clicked, the function handleClick should be called.


* **Knowing what you learned from the previous question, add code/markup to the `jsPracticeLab.html` file *so that* there is a button with the text `Spring Equinox 2019` on it somewhere on the page, and when that button is clicked, a text box containing the text `March 20, 2019` appears. (There's no function -- that I am aware of -- to automatically get this info, you've got to type it yourself.)**

Done. Lines 36-38 (function) and line 79 (button).

### The next few questions address the `jquerylib_submit_example.html` file.

* **Check out the file `jquerylib_submit_example.html`. This is an example of code that uses a package called `jQuery` (and this will need you to have an internet connection to run it properly, although the other file does not). Check out resources above for more on jQuery!**

* **When you enter input that isn't valid, you see an error that is red. Why is the error in red? Why is the response for valid inputs blue?**
The error message is red because it is tagged "class = error" and the style section dictates that things with that class are red. The valid response is tagged "good" which the style section indicates should be blue.

* **What is this line `var regex = /^[a-zA-Z]+$/;` helping with? And if you googled something to figure that out, what did you google, and what, briefly, did you learn? (If you didn't need to google, you can leave that out, but explain briefly what that line is helping the program do, anyway.)**
I think this is making everything lower case and allowing (or not allowing) certain characters. Going to Google "var regex = /^[a-zA-Z]+$/; javascript"

Okay, I was wrong. a-zA-A is the entire alphabet, capital or lower cased. And the +$/ is to allow spaces. So this is saying that when used as a test, var regex will be true for any input that is composed of only letters A-Z, capital or lower case, and spaces. Special characters (!@.,) and numbers would be false.

* **What's different about the syntax of conditional statements in JavaScript, compared to Python?**
The else statement is indented. The statements being compared are in parenthesis.

* **What do you think the `10000` refers to in the code `.fadeOut(10000)`?**
Time. Probably in milliseconds. Definitely not seconds.

* **What do you think is going on with the following code at the beginning of the program? Note that the most important thing to do for answering this question is to be thoughtful and clear, not to be absolutely correct:**

```js
$(document).ready(function(){
    $("form").submit(function(event){
```

I'm not entirely sure, but this is what I think is going on: document refers to the page is my browser and .ready(function) is from the jquery library to something. A Google search of ".ready(function) + jquery" indicates that .ready is a method that can be called on the document to make a function available after the page is loaded. So I think that means that the indented text below this line should still be available after the page is loaded. And I think that makes sense because I would want to be able to submit the form, as mentioned on the next line after the page has loaded in my browser. This is a bit different to the other forms that we have seen where submitting the form directs to a new page. In this case, the same document and the ability to submit the form again and again remains.

The second line is saying when the form is submitted to execute the following lines of code. The following lines of code are the conditional statements which check if the text entered in the form is considered valid or invalid.

* **Add some code to the `jquerylib_submit_example.html` file so that, if the input is valid and is specifically the text `hello`, rather than the visible output being `Nice!` in blue, the visible output should be `Hello to you too!`, also in blue, just like `Nice!` is.**
	* *HINT:* You'll have to make some changes to the conditional statement, and possibly look up some JavaScript conditional syntax. You'll also need to look carefully at what generates visible output right now.

Lines 24-25
