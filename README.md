# CodeClauseInternship_To-dolist
I'm thrilled to share that I have successfully completed the #CodeClauseInternship task, creating a dynamic To-Do List using HTML, CSS, and JavaScript! 📝💻
HTML Part:
Document Type Declaration (<!DOCTYPE html>):

Specifies the document type and version of HTML being used (HTML5 in this case).
**HTML Document Structure:**

<html lang="en">: Declares the document's language as English.
<head>: Contains metadata about the document, such as character set, viewport settings, and the title of the page.
<meta charset="UTF-8">: Sets the character set to UTF-8 (Unicode).
<meta name="viewport" content="width=device-width, initial-scale=1.0">: Defines the viewport settings for responsive design.
<title>To-Do List</title>: Sets the title of the HTML document.
<link rel="stylesheet" type="text/css" href="style.css">: Links an external stylesheet (CSS) file named "style.css" to apply styles to the HTML document.
Body Content:

**<body>: Contains the visible content of the HTML document.**
<div class="container">: Creates a container div to hold the entire content.
<div class="box">: Creates a box div inside the container.
<h2>To Do List</h2>: Heading displaying "To Do List".
<input type="text" placeholder="Writer here: " id="inputBx">: Input field for the user to type in tasks. It has an id attribute set to "inputBx" for JavaScript access.
<ul id="List"></ul>: Unordered list (ul) element with an id of "List" where the to-do list items will be displayed.
JavaScript Part:
Script Section:

**<script>: Contains JavaScript code for dynamic behavior.**
let inputBx = document.querySelector('#inputBx');: Selects the input element with the id "inputBx" and assigns it to the variable inputBx.
let list = document.querySelector("#List");: Selects the unordered list with the id "List" and assigns it to the variable list.
Event Listener:

inputBx.addEventListener("keyup", function(event){...}: Listens for keyup events on the input field. If the pressed key is "Enter," it calls the addItem function with the input value and clears the input field.
addItem Function:

let addItem = (inputValue) => {...}: Declares a function named addItem that takes an inputValue parameter.
let listItem = document.createElement("li");: Creates a new list item (li) element.
listItem.innerHTML = ${inputValue}<i></i>;: Sets the inner HTML of the list item with the input value and an empty italic element (<i></i>) for styling.
listItem.addEventListener("click", function(){...}: Listens for click events on the list item and toggles the "done" class to mark the task as completed or not.
listItem.querySelector("i").addEventListener("click", function(){...}: Listens for click events on the italic element inside the list item and removes the corresponding list item when clicked.
list.appendChild(listItem);: Appends the list item to the unordered list.
