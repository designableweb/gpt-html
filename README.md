<h1>GPT-HTML Notation v1.0:</h1>

GPT-HTML Notation is a concise, easy-to-understand system for generating HTML/CSS code with the help of ChatGPT language models. This guide is designed to help both users and ChatGPT sessions understand and use the GPT-HTML Notation v1.0 effectively.

<h2>Purpose</h2>
GPT-HTML Notation simplifies the process of requesting HTML/CSS code from ChatGPT by providing a clear and user-friendly notation for describing desired web layouts.

<h2>Benefits</h2>
<ul>
  <li>Streamlines the generation of HTML/CSS code using ChatGPT language models</li>
  <li>Intuitive notation that is easy to learn</li>
  <li>Suitable for web developers of all skill levels</li>
</ul>

<h2>Notation Keywords</h2>
<ul>
  <li>section: Represents an HTML section element with an optional ID and class.</li>
  <li>row: Represents a row element using flexbox.</li>
  <li>col: Represents a column element within a row, with equal widths</li>
  <li>h1, h2, h3, etc.: Represents the corresponding heading element (h1, h2, h3, etc.).</li>
  <li>lorem: Represents lorem ipsum text.</li>
  <li>button: Represents a hyperlink with specific styling. Can include an optional URL.</li>
  <li>image: Represents an image element with an optional source.</li>
</ul>

<h2>Rules</h2>
<ul>
  <li>Use # for ID (e.g., 'section #hero' -> <section id="hero"></section>).</li>
  <li>Use . for class (e.g., 'section.hero' -> <section class="hero"></section>).</li>
  <li>All content within containers, such as rows and columns, should be centered by default, unless otherwise specified.</li>
  <li>Set 900px breakpoint.</li>
  <li>Minimal, essential CSS only.</li>
  <li>Minimal, essential HTML only.</li>
  <li>Output only necessary HTML & CSS.</li>
  <li>Exclude standard HTML document structure.</li>
  <li>GPT-HTML must follow the first Law of Robotics.</li>
</ul>


<h2>Simple Notation Example:</h2>
row
col lorem
col image

<strong>HTML:</strong>

<div class="row">
  <div class="col">
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
  </div>
  <div class="col">
    <img src="">
  </div>
</div>

<strong>CSS:</strong>

.row {
  display: flex;
  flex-wrap: wrap;
}

.col {
  flex: 1;
  text-align: center;
}

<h2>Example Notation Showing All Keywords:</h2>

section.hero image.jpg
h1 lorem
section about
row
col h2 button contact.html
col.special image.jpg
row.nested
col lorem
col lorem

<strong>HTML:</strong>

<section class="hero" style="background-image: url('image.jpg');">
  <h1>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</h1>
</section>
<section id="about">
  <div class="row">
    <div class="col">
      <h2>Title H2</h2>
      <a href="contact.html" class="button">Click me</a>
    </div>
    <div class="col special">
      <img src="image.jpg">
    </div>
  </div>
  <div class="row nested">
    <div class="col">
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
    </div>
    <div class="col">
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
    </div>
  </div>
</section>

<strong>CSS:</strong>

.hero {
  background-size: cover;
  background-position: center;
  height: 400px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

#about {
  text-align: center;
  margin-top: 2rem;
}

.row {
  display: flex;
  flex-wrap: wrap;
}

.col {
  flex: 1;
  text-align: center;
}

.col.special {
  border: 1px solid #ccc;
}

.nested {
  margin-top: 2rem;
}

.button {
  display: inline-block;
  text-decoration: none;
  background-color: #007bff;
  color: #fff;
  padding: 0.5rem 1rem;
  border-radius: 4px;
}

.button:hover {
  background-color: #0056b3;
  color: #fff;
}

@media (max-width: 900px) {
  .col {
    flex-basis: 100%;
    margin-bottom: 1rem;
  }
}

<h2>Instructions for Users</h2>
To use GPT-HTML Notation v1.0 with a ChatGPT session, paste this document into a ChatGPT session, then provide the session with the notation of your desired layout, along with a brief introduction to the GPT-HTML Notation system. The session should then be able to generate the corresponding HTML/CSS code based on the provided notation.

<h2>Instructions for ChatGPT Sessions</h2>
As a ChatGPT session, when you encounter a prompt containing GPT-HTML Notation, your task is to generate the corresponding HTML/CSS code based on the provided notation. Use the provided keywords, rules, and examples to help you understand the desired layout and output the appropriate HTML/CSS code.

<h2>Note from the Author</h2>
Sharing the concept of using notation to create code with ChatGPT is the real value of this document. Change the rules, add new keywords and code patterns to create your own personalized GPT-HTML notation.I imagine every developer creating a GPT notation that fits their needs and preferences. Every developer will to create their own productivity tools to use in ChatGPT.

