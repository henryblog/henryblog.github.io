---
title: Resources for Javascript & jQuery
category: javascript jquery Wyncode
side_title2: ["JavaScript Loops, Arrays and Objects", "Second"]
treehouse:
  - top_title: JavaScript Basics
    content: "JavaScript is a programming language that drives the web: from front-end user interface design, to backend server-side programming, you'll find JavaScript at every stage of a web site and web application. In this course, you'll learn the fundamental programming concepts and syntax of the JavaScript programming language."
    link: https://teamtreehouse.com/library/javascript-basics
  - top_title: jQuery Basics
    content: "jQuery Basics covers why you'd want to use jQuery, what it is and how to include it in your projects. You'll build several projects over the course to give you the confidence to integrate jQuery in your own projects and add that level of flair and interactivity to any site you work on."
    link: https://teamtreehouse.com/library/jquery-basics
  - top_title: AJAX Basics
    content: "AJAX is an important front-end web technology that lets JavaScript communicate with a web server. It lets you load new content without leaving the current page, creating a better, faster experience for your web site's visitors. In this course, you'll learn how AJAX works and how you can use JavaScript to communicate with a web server."
    link: https://teamtreehouse.com/library/ajax-basics

books:
  - top_title: Eloquent JavaScript
    content: "This is a book about JavaScript, programming, and the wonders of the digital. You can read it online here, or get your own paperback copy of the book."
    link: http://eloquentjavascript.net/
    type: Book
  - top_title: Introduction To JavaScript
    content: Learn the fundamentals of JavaScript, the programming language of the Web.
    link: https://www.codecademy.com/learn/javascript
    type: Course
  - top_title: JavaScript For Cats
    content: "JavaScript is a programming language or, in other words, a means by which a computer is instructed to do things."
    link: http://jsforcats.com/
    type: Book
---


<ul class="list--divided">
  <h2>Treehouse Resources</h2>
  {% for trhouse in page.treehouse %}
    <li class="list-item">
      <div class="grid__col--12 flex-wrap">
        <div class="grid__col--4 no-padding">
          <a href="{{ trhouse.link }}" class="treeh-panel">
            <div class="treeh-panel-heading text-center centered" style="width:90%">
              {{ trhouse.top_title }}
            </div>
          </a>
        </div>
        <div class="grid__col--8">
          <h3>{{ trhouse.top_title }}</h3>
          <p>{{ trhouse.content }}</p>
          <span>
            <a href="{{ trhouse.link }}" class="btn btn__hover" title="">View Course</a>
          </span>
        </div>
      </div>
    </li>
  {% endfor %}
</ul>


<h2>JavaScript Tutorials</h2>
<div class="grid__col--12">
  {% for resource in page.books %}
    <div class="grid__col--4">
      <a href="{{ trhouse.link }}" class="book-panel">
        <div class="book-panel-heading text-center centered" style="width:90%">
          {{ resource.top_title }}
        </div>
      </a>
      <p>{{ resource.content }}</p>
      <span>
        <a href="{{ trhouse.link }}" class="btn btn__hover" title="">View {{resource.type}}</a>
      </span>
    </div>
  {% endfor %}
</div>