# From Start to Post: Goal

This is an assignment for Hacking History, a digital humanities course taught in the History Department at the University of Toronto. If you're a teacher, feel free to fork and repurpose for your own courses. If you're a student, keep reading!

You do not have to become a coder to do well in this course. However, you *will* have to be willing to explore technical skills that you might not otherwise develop as a humanities scholar. In this assignment, you will refresh your knowledge of *very basic* web coding skills and apply them to a simple problem. The goal of the assignment is to remind you of the basic technical knowledge that you will need for later assignments.


# Expectations

This assignment is graded pass/fail. You will only get credit if **all of your code runs as required.** To pass the assignment, you must:

-   successfully create a github repository and clone a local copy
-   complete all 3 problems of this assignment
-   commit your work to git as you go, so that a query of the git history will show multiple steps. Please note that git commits are timestamped and unique; they are an excellent defense against accusations of cheating, so please use them extensively.
-   push all your changes to Github


# Preparation

Please work your way through the following HTML and CSS resources (these are also listed in the syllabus):

-   [MDN: Getting Started with the Web](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web)
-   [MDN: Intro to HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML). This is a great, systematic introduction to the most important HTML elements.
-   [MDN: Learn HTML Pathway](https://developer.mozilla.org/en-US/docs/Learn/HTML#Modules). You won't need all of this, but a lot of it is interesting.
-   [MDN: Learn CSS Pathway](https://developer.mozilla.org/en-US/docs/Learn/CSS). Again, there is more here than you need, but big parts of it will be used in this assignment.


# Details

Presumably you already have an assignment link that will clone the repository for you. Now clone locally via the "Clone or Download" process [described here](https://help.github.com/articles/cloning-a-repository/), or just use [the VSCode git commands](https://code.visualstudio.com/docs/editor/versioncontrol#_cloning-a-repository). Do your work in VSCode, then push your repo to the cloud when you're ready.

Web pages are composed of three components: HTML, CSS, and Javascript. HTML provides the *structure and content* of a web page; CSS controls the *style of presentation*; and Javascript permits *dynamic modification* of both. In this assignment, we explore the first two components, HTML and CSS


## Problem 1: HTML Structure

Make sure you've read [intro to HTML overview](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started) and have explored enough to orient yourself when you run into difficulties.

In the directory `01`, find the file `01/letter.txt`. Your job is to convert this raw text into *structured HTML*. I've provided you with some starter code in `01/index.html`. Please make changes as follow:

-   Header:
    -   add the sender info in the appropriate `div` element. Wrap the information in a `<p>` element and divide lines with [<br> elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/br)
    -   add the date in the `<time>` element
    -   add the recipient info in the `recipient` div element, wrap in a `p` and divide w `br` as above.
    -   make sure that both email addresses are [working mailto: links](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#E-mail_links)
-   Main Text
    -   add the text of the greeting line ("Dear Prof&#x2026;") to the `div.greeting` element
    -   add the main text of the letter to the `div.text` element. Separate into paragraphs with `<p>` elements, but also note:
    -   The lines reading `Assignments`, `Lectures` and `Project` should be `<h1>` elements rather than `<p>` elements
    -   The lines starting with `- A...` should be made into [list elements in an unordered list](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#Unordered)
    -   add the closing (Sincerely,&#x2026; yr name) to the&#x2026;. wait for it&#x2026; that's right, to the `div.closing` element
-   Footer:
    -   Add the motto ("Perpetuis&#x2026;") to the `footer` element

If you've passed all the tests, then you should be fine!


## Problem 2: Basic Styling

CSS is an enormous topic, so it will be easy to get lost. In this problem we deal with a few basic CSS properties, mostly affecting fonts, colors, and spacing. Start with the well-structured HTML in `index.html`, to which very little styling has been applied so far.

We want to make the final page look something like this image:

[./02/ursula.png](./02/plague.png)

Please do the following:

-   set the default font-family for the whole page to `"Roboto", sans-serif`, using the `html` selector at the top of the file.
-   set the maximum width of `main` to `50rem` (we use a mixture of `px` and `rem` in this assignment!)
-   add a border radius of 10px to `main`
-   add a background color to both `header` and `footer`. Make it the same color!
-   add some padding ( 5px) to the top of `header`
-   add margins of 10px to the left and right of `article`, and set the `display` to `flow-root` to fix the old problem of uncleared floats.
-   give the `img` inside `article` a maximum width of `15rem`; also float it left; give it a visible border with a radius of at least 5px, and add a margin o n the right side to separate it from the text
-   make sure the minimum height of `footer` is at lest 5rem


## Problem 3: Post

OK, you've had a little practice, and you should now be ready to write a short post in pure HTML! Compose a brief statement (approximately 200 words) in HTML, arguing in favour of your preferred class project idea. You will write this post in `./03/index.html`, and style it in `./03/style.css`

**index.html\*** should contain, at a minimum, the following elements:

-   an `<article>` tag, which contains all of the elements mentioned below
-   a `<header>` element, inside of which there should also be:
    -   an `<h1>` element with the figure's name
    -   an `<h2>` element containing the text `by <span class="author">Your Name</span>` and any other "byline" information you would like to include
-   a `<section>` element with class `main`, containing your main content
-   an `<img>` tag **within** the main section. The image should be a picture of the historical figure, or related to the historical event or process.
-   a `<section>` element with class `sources`.
-   inside your sources section, a `<ul>` element containing at least two `<li>` elements, each of which lists one source that you used in writing your blog post. The title of the source should be a hyperlink with `href` attribute linking back to the source. If your source is a print book or article, the link should point to the source's listing in the library catalog. In the extremely unlikely event that the source is not among the library's holdings, use an Amazon or Google Scholar link instead.

**style.css** should style the page. Since you come to this assignment with very different levels of knowledge, I will leave the specifics up to you and enjoy the results!


# Handing in

Simply push your changes to Github and I will see them!
