Calculator
==========

[![Join the chat at https://gitter.im/unioncollege-webtech/calculator](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/unioncollege-webtech/calculator?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Exercise your DOM skills to build functional calculator with JavaScript.


Description
-----------

Use DOM methods to create functional calculator that has buttons for the numbers
0–9 as well as for some basic operators for addition (+), subtraction (-), 
multiplication (* or x), division (/), and equals (=).

In addition to those buttons, the calculator should have a display which 
displays the numbers or operators pressed by the user. When the user presses
equals (=), the calculator should evaluate the math expression and update the
display with the result.

For this exercise, create *and style* a basic functional calculator purely with
JavaScript using the [DOM API]. Use [`document.createElement(tagname)`][document.createElement]
to create the [`button` elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/button)
and [`document.body.appendChild(element)`][node.appendChild]
to add them to the page. Use [`element.addEventListener`][element.addEventListener]
to listen to 'click' events on the buttons. When the 'click' event fires, update
the display and/or evaluate the math expression based on the button that was 
clicked (see [`event.currentTarget`][event.currentTarget] or
[`event.target`][event.target]).

Almost any element could be used for the calculator's display. An [`input`][input]
would work well, but it could just as well be [`div`][div], [`span`][span], or
[`p`][p].

If you use the `input` element, use the [`value`][input.value] property to 
update the display. If you use any other element the [`textContent`][textContent]
property should be used.

### Evaluating the result

To evaluate the result, use the math.js library ([mathjs.org][math.js]) by
calling [`math.eval(expression)`][math.eval]. The math.js library should be
loaded on the page before calculator.js.

### Styling the calculator

Please add at least basic styles to improve the usability of the calculator. The
styles should lay out the calculator buttons in a logical and organized manner.
Consider making the calculator usable on mobile devices as well.

### Additional functionality

Feel free to add additional operators or complex functionality for the
calculator. Math.js supports a wide range of operators and [complex expressions](http://mathjs.org/docs/expressions/syntax.html).


Completing and submitting the assignment
----------------------------------------

- To begin, [**fork** this repository](https://guides.github.com/activities/forking/).
- [Create a new Cloud9 workspace](https://docs.c9.io/docs/setting-up-github-workspace)
  from your new repository.
  - Alternatively, you may [**clone**](http://gitref.org/creating/#clone) your
    new repository to your computer by running:

        git clone https://github.com/YOUR_GITHUB_USERNAME/calculator

- After cloning (in Cloud9 or on your computer), check out the “**gh-pages**”
  branch by running:

        git checkout gh-pages

- Modify the files and [**commit**](http://gitref.org/basic/#commit) changes to complete your solution.
- Run `node test` to verify that all tests pass.
- [Push](http://gitref.org/remotes/#push)/sync the changes up to GitHub. Your assignment will now be visible at [http://YOUR_GITHUB_USERNAME.github.io/calculator/](http://unioncollege-webtech.github.io/calculator/).
- [Create a pull request](https://help.github.com/articles/creating-a-pull-request) on the original repository to turn in the assignment.
- [Create a separate branch](http://gitref.org/branching/#branch) for the extra credit options.

You are also welcome commit, push, and create a pull request **before** you’ve 
completed your solution. You can ask questions or request feedback there in your
pull request. Just mention `@barberboy` in your comments to get my attention.


References
----------

* [`document.createElement`][document.createElement]
* [`document.createTextNode`][document.createTextNode]
* [`node.appendChild`][node.appendChild]
* [`element.addEventListener`][element.addEventListener]
* [`event.currentTarget`][event.currentTarget]
* [`event.target`][event.target]
* [`button` element][button]
* [`input` element][input]
* [`div` element][div]
* [`span` element][span]
* [`p` element][p]
* [`textContent`][textContent] property

[document.createElement]: https://developer.mozilla.org/en-US/docs/Web/API/Document/createElement
[document.createTextNode]: https://developer.mozilla.org/en-US/docs/Web/API/Document/createTextNode
[node.appendChild]: https://developer.mozilla.org/en-US/docs/Web/API/Node/appendChild
[element.addEventListener]: https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/addEventListener
[event.currentTarget]: https://developer.mozilla.org/en-US/docs/Web/API/Event/currentTarget
[event.target]: https://developer.mozilla.org/en-US/docs/Web/API/Event/target
[button]: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/button
[input]: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input
[input.value]: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input#attr-value
[textContent]: https://developer.mozilla.org/en-US/docs/Web/API/Node/textContent
[div]: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/div
[span]: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/span
[p]: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/p
[DOM API]: https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction

[math.js]: http://mathjs.org
[math.eval]: http://mathjs.org/docs/expressions/parsing.html#eval