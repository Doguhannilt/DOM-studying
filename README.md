<h1>Document Object Model (DOM) Documentation</h1>

<section>
<h2>1. What is DOM?</h2>
<p>
The Document Object Model (DOM) is a cross-platform and language-independent interface that treats an XML or HTML document as a tree structure. It represents the structure of a document as a tree of objects, where each object corresponds to a part of the document, such as elements, attributes, and text. The DOM provides a way to interact with HTML and XML documents using a programming language like JavaScript.
</p>
</section>

<section>
<h2>2. DOM Syntax</h2>
<h3>Selecting Elements</h3>
<pre><code>
// getElementById
let element = document.getElementById("myElement");

// getElementsByClassName
let elements = document.getElementsByClassName("myClass");

// querySelector
let element = document.querySelector("#myElement");
</code></pre>

<h3>Manipulating Elements</h3>
<pre><code>
// Changing Text Content
element.textContent = "New Text Content";

// Changing Styles
element.style.color = "red";

// Creating Elements
let newElement = document.createElement("div");
</code></pre>

<h3>Events</h3>
<pre><code>
// Click Event
element.addEventListener("click", function() {
// Your code here
});

// Mouseover Event
element.addEventListener("mouseover", function() {
// Your code here
});

// Input Event
inputElement.addEventListener("input", function() {
console.log("Input value changed:", this.value);
});
</code></pre>
</section>

<section>
<h2>3. Why do we use DOM?</h2>
<p>
The DOM allows developers to dynamically manipulate the content and structure of web documents. It enables the creation of interactive and dynamic web pages by providing a way to:
</p>
<ul>
<li>Access and modify document content.</li>
<li>Respond to user interactions (events).</li>
<li>Create, delete, and modify elements.</li>
</ul>
</section>

<section>
<h2>4. Examples</h2>

<h3>Example 1: Changing Text and Styles</h3>
<pre><code>
let heading = document.getElementById("myHeading");
heading.textContent = "New Heading";
heading.style.color = "blue";
</code></pre>

<h3>Example 2: Handling Click Event</h3>
<pre><code>
let button = document.getElementById("myButton");
button.addEventListener("click", function() {
alert("Button Clicked!");
});
</code></pre>

<h3>Example 3: Creating and Appending Elements</h3>
<pre><code>
let newDiv = document.createElement("div");
newDiv.textContent = "New Element";
document.body.appendChild(newDiv);
</code></pre>
</section>
