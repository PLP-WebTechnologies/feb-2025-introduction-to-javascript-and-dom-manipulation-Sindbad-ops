# Introduction to JavaScript and DOM Manipulation

## Objectives

Write basic JavaScript functions.
Manipulate the DOM dynamically.
Respond to user interactions.

## Instructions

- Create a script.js file and link it to a HTML.
- Structure the document using DOCTYPE, html, head, and body.

>[!NOTE]
>  - Write JavaScript that:
>  - Changes text content dynamically.
>  - Modifies CSS styles via JavaScript.
>  - Adds or removes an element when a button is clicked.


# Tasks
- Create a well-structured HTML5 document.
- Use at least 5 different HTML elements.
- Ensure semantic correctness.

Happy Coding! 💻✨


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Webpage</title>
    <style>
        .hidden {
            display: none;
        }
        .highlight {
            color: red;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1 id="title">Welcome to My Interactive Webpage!</h1>
    
    <button id="changeTextButton">Change Text</button>
    <button id="changeStyleButton">Change Style</button>
    <button id="toggleElementButton">Toggle Element</button>

    <div id="newElement" class="hidden">
        <p>This is a new element added dynamically!</p>
    </div>

    <script>
        // Change text content dynamically
        const changeTextButton = document.getElementById("changeTextButton");
        const title = document.getElementById("title");

        changeTextButton.addEventListener("click", () => {
            title.textContent = "Text Changed! JavaScript is Awesome!";
        });

        // Modify CSS styles via JavaScript
        const changeStyleButton = document.getElementById("changeStyleButton");

        changeStyleButton.addEventListener("click", () => {
            title.classList.toggle("highlight");
        });

        // Add or remove an element
        const toggleElementButton = document.getElementById("toggleElementButton");
        const newElement = document.getElementById("newElement");

        toggleElementButton.addEventListener("click", () => {
            newElement.classList.toggle("hidden");
        });
    </script>
</body>
</html>

