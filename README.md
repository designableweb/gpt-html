<h1>GPT-HTML Notation v1.0:</h1>

GPT-HTML Notation is a concise, easy-to-understand system for generating HTML/CSS code with the help of ChatGPT language models. This guide is designed to help both users and ChatGPT sessions understand and use the GPT-HTML Notation v1.0 effectively.

<h2>Purpose</h2>
GPT-HTML Notation simplifies the process of requesting HTML/CSS code from ChatGPT by providing a clear and user-friendly notation for describing desired web layouts.

<h2>Benefits</h2>
Streamlines the generation of HTML/CSS code using ChatGPT language models
Intuitive notation that is easy to learn
Suitable for web developers of all skill levels
Keywords and Usage
Below are the keywords supported by GPT-HTML Notation v1.0:

<h2>Notation Keywords</h2>
section: Represents an HTML section element with an optional ID and class.
row: Represents a row element using flexbox.
col: Represents a column element within a row, with equal widths
h1, h2, h3, etc.: Represents the corresponding heading element (h1, h2, h3, etc.).
lorem: Represents lorem ipsum text.
button: Represents a hyperlink with specific styling. Can include an optional URL.
image: Represents an image element with an optional source.

<h2>Rules</h2>
Use # for ID (e.g., 'section #hero' -> <section id="hero"></section>).
Use . for class (e.g., 'section.hero' -> <section class="hero"></section>).
All content within containers, such as rows and columns, should be centered by default, unless otherwise specified.
Set 900px breakpoint.
Minimal, essential CSS only.
Minimal, essential HTML only.
Output only necessary HTML & CSS.
Exclude standard HTML document structure.
GPT-HTML must follow the first Law of Robotics

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

