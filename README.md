<h1 align="center">Front End Interview Handbook</h1>

<div align="center">
  <a href="https://dribbble.com/shots/3831443-Tech-Interview-Handbook">
    <img src="https://cdn.rawgit.com/yangshun/front-end-interview-handbook/f4d3132f/assets/book.svg" alt="Front End Interview Handbook" width="400"/>
    </a>
  <br>
  <p>
    <em>Credits: <a href="https://dribbble.com/shots/3831443-Tech-Interview-Handbook">Illustration</a> by <a href="https://dribbble.com/yangheng">@yangheng</a>
    </em>
  </p>
</div>

## What is this?

Unlike typical software engineer job interviews, front-end job interviews have less emphasis on algorithms and have more questions on intricate knowledge and expertise about the domain — HTML, CSS, JavaScript, just to name a few areas.

While there are some existing resources to help front end developers in preparing for interviews, they aren't as abundant as materials for a software engineer interview. Among the existing resources, probably the most helpful question bank would be [Front-end Developer Interview Questions](https://github.com/h5bp/Front-end-Developer-Interview-Questions). Unfortunately, I couldn't find many complete and satisfactory answers for these questions online, hence here is my attempt at answering them. Being an open source repository, the project can live on with the support of the community as the state of web evolves.

## Looking for Generic Interview Preparation?

You might be interested in the [Tech Interview Handbook](https://github.com/yangshun/tech-interview-handbook) which has helpful content on general coding interviews such as algorithms, behavioral questions and an [interview cheatsheet](https://github.com/yangshun/tech-interview-handbook/blob/master/preparing/cheatsheet.md)!

## Table of Contents

**[HTML Questions](#html-questions)**

* [What does a doctype do?](#what-does-a-doctype-do)
* [How do you serve a page with content in multiple languages?](#how-do-you-serve-a-page-with-content-in-multiple-languages)
* [What kind of things must you be wary of when design or developing for multilingual sites?](#what-kind-of-things-must-you-be-wary-of-when-designing-or-developing-for-multilingual-sites)
* [What are `data-` attributes good for?](#what-are-data--attributes-good-for)
* [Consider HTML5 as an open web platform. What are the building blocks of HTML5?](#consider-html5-as-an-open-web-platform-what-are-the-building-blocks-of-html5)
* [Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.](#describe-the-difference-between-a-cookie-sessionstorage-and-localstorage)
* [Describe the difference between `<script>`, `<script async>` and `<script defer>`.](#describe-the-difference-between-script-script-async-and-script-defer)
* [Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?](#why-is-it-generally-a-good-idea-to-position-css-links-between-headhead-and-js-scripts-just-before-body-do-you-know-any-exceptions)
* [What is progressive rendering?](#what-is-progressive-rendering)
* [Why you would use a `srcset` attribute in an image tag? Explain the process the browser uses when evaluating the content of this attribute.](#why-you-would-use-a-srcset-attribute-in-an-image-tag-explain-the-process-the-browser-uses-when-evaluating-the-content-of-this-attribute)
* [Have you used different HTML templating languages before?](#have-you-used-different-html-templating-languages-before)

**[CSS Questions](#css-questions)**

* [What is CSS selector specificity and how does it work?](#what-is-css-selector-specificity-and-how-does-it-work)
* [What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why?](#whats-the-difference-between-resetting-and-normalizing-css-which-would-you-choose-and-why)
* [Describe `float`s and how they work.](#describe-floats-and-how-they-work)
* [Describe z-index and how stacking context is formed.](#describe-z-index-and-how-stacking-context-is-formed)
* [Describe BFC (Block Formatting Context) and how it works.](#describe-block-formatting-context-bfc-and-how-it-works)
* [What are the various clearing techniques and which is appropriate for what context?](#what-are-the-various-clearing-techniques-and-which-is-appropriate-for-what-context)
* [Explain CSS sprites, and how you would implement them on a page or site.](#explain-css-sprites-and-how-you-would-implement-them-on-a-page-or-site)
* [How would you approach fixing browser-specific styling issues?](#how-would-you-approach-fixing-browser-specific-styling-issues)
* [How do you serve your pages for feature-constrained browsers? What techniques/processes do you use?](#how-do-you-serve-your-pages-for-feature-constrained-browsers-what-techniquesprocesses-do-you-use)
* [What are the different ways to visually hide content (and make it available only for screen readers)?](#what-are-the-different-ways-to-visually-hide-content-and-make-it-available-only-for-screen-readers)
* [Have you ever used a grid system, and if so, what do you prefer?](#have-you-ever-used-a-grid-system-and-if-so-what-do-you-prefer)
* [Have you used or implemented media queries or mobile specific layouts/CSS?](#have-you-used-or-implemented-media-queries-or-mobile-specific-layoutscss)
* [Are you familiar with styling SVG?](#are-you-familiar-with-styling-svg)
* [Can you give an example of an @media property other than screen?](#can-you-give-an-example-of-an-media-property-other-than-screen)
* [What are some of the "gotchas" for writing efficient CSS?](#what-are-some-of-the-gotchas-for-writing-efficient-css)
* [What are the advantages/disadvantages of using CSS preprocessors?](#what-are-the-advantagesdisadvantages-of-using-css-preprocessors)
* [Describe what you like and dislike about the CSS preprocessors you have used.](#describe-what-you-like-and-dislike-about-the-css-preprocessors-you-have-used)
* [How would you implement a web design comp that uses non-standard fonts?](#how-would-you-implement-a-web-design-comp-that-uses-non-standard-fonts)
* [Explain how a browser determines what elements match a CSS selector.](#explain-how-a-browser-determines-what-elements-match-a-css-selector)
* [Describe pseudo-elements and discuss what they are used for.](#describe-pseudo-elements-and-discuss-what-they-are-used-for)
* [Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.](#explain-your-understanding-of-the-box-model-and-how-you-would-tell-the-browser-in-css-to-render-your-layout-in-different-box-models)
* [What does `* { box-sizing: border-box; }` do? What are its advantages?](#what-does---box-sizing-border-box--do-what-are-its-advantages)
* [What is the CSS `display` property and can you give a few examples of its use?](#what-is-the-css-display-property-and-can-you-give-a-few-examples-of-its-use)
* [What's the difference between `inline` and `inline-block`?](#whats-the-difference-between-inline-and-inline-block)
* [What's the difference between a `relative`, `fixed`, `absolute` and `static`ally positioned element?](#whats-the-difference-between-a-relative-fixed-absolute-and-static-ally-positioned-element)
* [What existing CSS frameworks have you used locally, or in production? How would you change/improve them?](#what-existing-css-frameworks-have-you-used-locally-or-in-production-how-would-you-changeimprove-them)
* [Have you played around with the new CSS Flexbox or Grid specs?](#have-you-played-around-with-the-new-css-flexbox-or-grid-specs)
* [Can you explain the difference between coding a web site to be responsive versus using a mobile-first strategy?](#can-you-explain-the-difference-between-coding-a-web-site-to-be-responsive-versus-using-a-mobile-first-strategy)
* [Have you ever worked with retina graphics? If so, when and what techniques did you use?](#have-you-ever-worked-with-retina-graphics-if-so-when-and-what-techniques-did-you-use)
* [Is there any reason you'd want to use `translate()` instead of `absolute` positioning, or vice-versa? And why?](#is-there-any-reason-youd-want-to-use-translate-instead-of-absolute-positioning-or-vice-versa-and-why)

**[JS Questions](#js-questions)**

* [Explain event delegation](#explain-event-delegation)
* [Explain how `this` works in JavaScript](#explain-how-this-works-in-javascript)
* [Explain how prototypal inheritance works](#explain-how-prototypal-inheritance-works)
* [What do you think of AMD vs CommonJS?](#what-do-you-think-of-amd-vs-commonjs)
* [Explain why the following doesn't work as an IIFE: `function foo(){ }();`. What needs to be changed to properly make it an IIFE?](#explain-why-the-following-doesnt-work-as-an-iife-function-foo--what-needs-to-be-changed-to-properly-make-it-an-iife)
* [What's the difference between a variable that is: `null`, `undefined` or undeclared? How would you go about checking for any of these states?](#whats-the-difference-between-a-variable-that-is-null-undefined-or-undeclared-how-would-you-go-about-checking-for-any-of-these-states)
* [What is a closure, and how/why would you use one?](#what-is-a-closure-and-howwhy-would-you-use-one)
* [Can you describe the main difference between a `.forEach` loop and a `.map()` loop and why you would pick one versus the other?](#can-you-describe-the-main-difference-between-a-foreach-loop-and-a-map-loop-and-why-you-would-pick-one-versus-the-other)
* [What's a typical use case for anonymous functions?](#whats-a-typical-use-case-for-anonymous-functions)
* [How do you organize your code? (module pattern, classical inheritance?)](#how-do-you-organize-your-code-module-pattern-classical-inheritance)
* [What's the difference between host objects and native objects?](#whats-the-difference-between-host-objects-and-native-objects)
* [Difference between: function `Person(){}`, `var person = Person()`, and `var person = new Person()`?](#difference-between-function-person-var-person--person-and-var-person--new-person)
* [What's the difference between `.call` and `.apply`?](#whats-the-difference-between-call-and-apply)
* [Explain `Function.prototype.bind`.](#explain-functionprototypebind)
* [When would you use `document.write()`?](#when-would-you-use-documentwrite)
* [What's the difference between feature detection, feature inference, and using the UA string?](#whats-the-difference-between-feature-detection-feature-inference-and-using-the-ua-string)
* [Explain Ajax in as much detail as possible.](#explain-ajax-in-as-much-detail-as-possible)
* [What are the advantages and disadvantages of using Ajax?](#what-are-the-advantages-and-disadvantages-of-using-ajax)
* [Explain how JSONP works (and how it's not really Ajax).](#explain-how-jsonp-works-and-how-its-not-really-ajax)
* [Have you ever used JavaScript templating? If so, what libraries have you used?](#have-you-ever-used-javascript-templating-if-so-what-libraries-have-you-used)
* [Explain "hoisting".](#explain-hoisting)
* [Describe event bubbling.](#describe-event-bubbling)
* [What's the difference between an "attribute" and a "property"?](#whats-the-difference-between-an-attribute-and-a-property)
* [Why is extending built-in JavaScript objects not a good idea?](#why-is-extending-built-in-javascript-objects-not-a-good-idea)
* [Difference between document `load` event and document `DOMContentLoaded` event?](#difference-between-document-load-event-and-document-domcontentloaded-event)
* [What is the difference between `==` and `===`?](#what-is-the-difference-between--and-)
* [Explain the same-origin policy with regards to JavaScript.](#explain-the-same-origin-policy-with-regards-to-javascript)
* [Make this work: `duplicate([1,2,3,4,5]); // [1,2,3,4,5,1,2,3,4,5]`](#make-this-work)
* [Why is it called a Ternary expression, what does the word "Ternary" indicate?](#why-is-it-called-a-ternary-expression-what-does-the-word-ternary-indicate)
* [What is "use strict";? what are the advantages and disadvantages to using it?](#what-is-use-strict-what-are-the-advantages-and-disadvantages-to-using-it)
* [Create a for loop that iterates up to 100 while outputting "fizz" at multiples of 3, "buzz" at multiples of 5 and "fizzbuzz" at multiples of 3 and 5](#create-a-for-loop-that-iterates-up-to-100-while-outputting-fizz-at-multiples-of-3-buzz-at-multiples-of-5-and-fizzbuzz-at-multiples-of-3-and-5)
* [Why is it, in general, a good idea to leave the global scope of a website as-is and never touch it?](#why-is-it-in-general-a-good-idea-to-leave-the-global-scope-of-a-website-as-is-and-never-touch-it)
* [Why would you use something like the `load` event? Does this event have disadvantages? Do you know any alternatives, and why would you use those?](#why-would-you-use-something-like-the-load-event-does-this-event-have-disadvantages-do-you-know-any-alternatives-and-why-would-you-use-those)
* [Explain what a single page app is and how to make one SEO-friendly.](#explain-what-a-single-page-app-is-and-how-to-make-one-seo-friendly)
* [What is the extent of your experience with Promises and/or their polyfills?](#what-is-the-extent-of-your-experience-with-promises-andor-their-polyfills)
* [What are the pros and cons of using Promises instead of callbacks?](#what-are-the-pros-and-cons-of-using-promises-instead-of-callbacks)
* [What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?](#what-are-some-of-the-advantagesdisadvantages-of-writing-javascript-code-in-a-language-that-compiles-to-javascript)
* [What tools and techniques do you use debugging JavaScript code?](#what-tools-and-techniques-do-you-use-for-debugging-javascript-code)
* [What language constructions do you use for iterating over object properties and array items?](#what-language-constructions-do-you-use-for-iterating-over-object-properties-and-array-items)
* [Explain the difference between mutable and immutable objects.](#explain-the-difference-between-mutable-and-immutable-objects)
* [Explain the difference between synchronous and asynchronous functions.](#explain-the-difference-between-synchronous-and-asynchronous-functions)
* [What is event loop? What is the difference between call stack and task queue?](#what-is-event-loop-what-is-the-difference-between-call-stack-and-task-queue)
* [Explain the differences on the usage of `foo` between `function foo() {}` and `var foo = function() {}`](#explain-the-differences-on-the-usage-of-foo-between-function-foo--and-var-foo--function-)
* [What are the differences between variables created using `let`, `var` or `const`?](#what-are-the-differences-between-variables-created-using-let-var-or-const)
* [What are the differences between ES6 class and ES5 function constructors?](#what-are-the-differences-between-es6-class-and-es5-function-constructors)
* [Can you offer a use case for the new arrow => function syntax? How does this new syntax differ from other functions?](#can-you-offer-a-use-case-for-the-new-arrow--function-syntax-how-does-this-new-syntax-differ-from-other-functions)
* [What advantage is there for using the arrow syntax for a method in a constructor?](#what-advantage-is-there-for-using-the-arrow-syntax-for-a-method-in-a-constructor)
* [What is the definition of a higher-order function?](#what-is-the-definition-of-a-higher-order-function)
* [Can you give an example for destructuring an object or an array?](#can-you-give-an-example-for-destructuring-an-object-or-an-array)
* [ES6 Template Literals offer a lot of flexibility in generating strings, can you give an example?](#es6-template-literals-offer-a-lot-of-flexibility-in-generating-strings-can-you-give-an-example)
* [Can you give an example of a curry function and why this syntax offers an advantage?](#can-you-give-an-example-of-a-curry-function-and-why-this-syntax-offers-an-advantage)
* [What are the benefits of using spread syntax and how is it different from rest syntax?](#what-are-the-benefits-of-using-spread-syntax-and-how-is-it-different-from-rest-syntax)
* [How can you share code between files?](#how-can-you-share-code-between-files)
* [Why you might want to create static class members?](#why-you-might-want-to-create-static-class-members)

---

## HTML Questions

Answers to [Front-end Job Interview Questions - HTML Questions](https://github.com/h5bp/Front-end-Developer-Interview-Questions#html-questions). Pull requests for suggestions and corrections are welcome!

---

### What does a `DOCTYPE` do?

`DOCTYPE` is an abbreviation for “document type”. It is a declaration used in HTML to distinguish between standards mode and [quirks mode](https://quirks.spec.whatwg.org/#history). Its presence tells the browser to render the web page in standards mode.

Moral of the story - just add `<!DOCTYPE html>` at the start of your page.

###### References

* https://stackoverflow.com/questions/7695044/what-does-doctype-html-do
* https://www.w3.org/QA/Tips/Doctype
* https://quirks.spec.whatwg.org/#history

---

### How do you serve a page with content in multiple languages?

The question is a little vague, I will assume that it is asking about the most common case, which is how to serve a page with content available in multiple languages, but the content within the page should be displayed only in one consistent language.

When an HTTP request is made to a server, the requesting user agent usually sends information about language preferences, such as in the `Accept-Language` header. The server can then use this information to return a version of the document in the appropriate language if such an alternative is available. The returned HTML document should also declare the `lang` attribute in the `<html>` tag, such as `<html lang="en">...</html>`.

In the back end, the HTML markup will contain `i18n` placeholders and content for the specific language stored in YML or JSON formats. The server then dynamically generates the HTML page with content in that particular language, usually with the help of a back end framework.

###### References

* https://www.w3.org/International/getting-started/language

---

### What kind of things must you be wary of when designing or developing for multilingual sites?

* Use `lang` attribute in your HTML.
* Directing users to their native language - Allow a user to change his country/language easily without hassle.
* Text in images is not a scalable approach - Placing text in an image is still a popular way to get good-looking, non-system fonts to display on any computer. However to translate image text, each string of text will need to have it's a separate image created for each language. Anything more than a handful of replacements like this can quickly get out of control.
* Restrictive words / sentence length - Some content can be longer when written in another language. Be wary of layout or overflow issues in the design. It's best to avoid designing where the amount of text would make or break a design. Character counts come into play with things like headlines, labels, and buttons. They are less of an issue with free flowing text such as body text or comments.
* Be mindful of how colors are perceived - Colors are perceived differently across languages and cultures. The design should use color appropriately.
* Formatting dates and currencies - Calendar dates are sometimes presented in different ways. Eg. "May 31, 2012" in the U.S. vs. "31 May 2012" in parts of Europe.
* Do not concatenate translated strings - Do not do anything like `"The date today is " + date`. It will break in languages with different word order. Use a template string with parameters substitution for each language instead. For example, look at the following two sentences in English and Chinese respectively: `I will travel on {% date %}` and `{% date %} 我会出发`. Note that the position of the variable is different due to grammar rules of the language.
* Language reading direction - In English, we read from left-to-right, top-to-bottom, in traditional Japanese, text is read up-to-down, right-to-left.

###### References

* https://www.quora.com/What-kind-of-things-one-should-be-wary-of-when-designing-or-developing-for-multilingual-sites

---

### What are `data-` attributes good for?

Before JavaScript frameworks became popular, front end developers used `data-` attributes to store extra data within the DOM itself, without other hacks such as non-standard attributes, extra properties on the DOM. It is intended to store custom data private to the page or application, for which there are no more appropriate attributes or elements.

These days, using `data-` attributes is not encouraged. One reason is that users can modify the data attribute easily by using inspect element in the browser. The data model is better stored within JavaScript itself and stay updated with the DOM via data binding possibly through a library or a framework.

###### References

* http://html5doctor.com/html5-custom-data-attributes/
* https://www.w3.org/TR/html5/dom.html#embedding-custom-non-visible-data-with-the-data-*-attributes

---

### Consider HTML5 as an open web platform. What are the building blocks of HTML5?

* Semantics - Allowing you to describe more precisely what your content is.
* Connectivity - Allowing you to communicate with the server in new and innovative ways.
* Offline and storage - Allowing webpages to store data on the client-side locally and operate offline more efficiently.
* Multimedia - Making video and audio first-class citizens in the Open Web.
* 2D/3D graphics and effects - Allowing a much more diverse range of presentation options.
* Performance and integration - Providing greater speed optimization and better usage of computer hardware.
* Device access - Allowing for the usage of various input and output devices.
* Styling - Letting authors write more sophisticated themes.

###### References

* https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5

---

### Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.

All the above mentioned technologies are key-value storage mechanisms on the client side. They are only able to store values as strings.

|                                        | `cookie`                                                 | `localStorage` | `sessionStorage` |
| -------------------------------------- | -------------------------------------------------------- | -------------- | ---------------- |
| Initiator                              | Client or server. Server can use `Set-Cookie` header     | Client         | Client           |
| Expiry                                 | Manually set                                             | Forever        | On tab close     |
| Persistent across browser sessions     | Depends on whether expiration is set                     | Yes            | No               |
| Have domain associated                 | Yes                                                      | No             | No               |
| Sent to server with every HTTP request | Cookies are automatically being sent via `Cookie` header | No             | No               |
| Capacity (per domain)                  | 4kb                                                      | 5MB            | 5MB              |
| Accessibility                          | Any window                                               | Any window     | Same tab         |

###### References

* https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies
* http://tutorial.techaltum.com/local-and-session-storage.html

---

### Describe the difference between `<script>`, `<script async>` and `<script defer>`.

* `<script>` - HTML parsing is blocked, the script is fetched and executed immediately, HTML parsing resumes after the script is executed.
* `<script async>` - The script will be fetched in parallel to HTML parsing and executed as soon as it is available (potentially before HTML parsing completes). Use `async` when the script is independent of any other scripts on the page, for example analytics.
* `<script defer>` - The script will be fetched in parallel to HTML parsing and executed when the page has finished parsing. If there are multiple of them, each deferred script is executed in the order they were encoun­tered in the document. If a script relies on a fully-parsed DOM, the `defer` attribute will be useful in ensuring that the HTML is fully parsed before executing. There's not much difference from putting a normal `<script>` at the end of `<body>`. A deferred script must not contain `document.write`.

Note: The `async` and `defer` attrib­utes are ignored for scripts that have no `src` attribute.

###### References

* http://www.growingwiththeweb.com/2014/02/async-vs-defer-attributes.html
* https://stackoverflow.com/questions/10808109/script-tag-async-defer
* https://bitsofco.de/async-vs-defer/

---

### Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?

**Placing `<link>`s in the `<head>`**

Putting `<link>`s in the head is part of the specification. Besides that, placing at the top allows the page to render progressively which improves user experience. The problem with putting stylesheets near the bottom of the document is that it prohibits progressive rendering in many browsers, including Internet Explorer. Some browsers block rendering to avoid having to repaint elements of the page if their styles change. The user is stuck viewing a blank white page. It prevents the flash of unstyled contents.

**Placing `<script>`s just before `</body>`**

`<script>`s block HTML parsing while they are being downloaded and executed. Downloading the scripts at the bottom will allow the HTML to be parsed and displayed to the user first.

An exception for positioning of `<script>`s at the bottom is when your script contains `document.write()`, but these days it's not a good practice to use `document.write()`. Also, placing `<script>`s at the bottom means that the browser cannot start downloading the scripts until the entire document is parsed. One possible workaround is to put `<script>` in the `<head>` and use the `defer` attribute.

###### References

* https://developer.yahoo.com/performance/rules.html#css_top

---

### What is progressive rendering?

Progressive rendering is the name given to techniques used to improve performance of a webpage (in particular, improve perceived load time) to render content for display as quickly as possible.

It used to be much more prevalent in the days before broadband internet but it is still useful in modern development as mobile data connections are becoming increasingly popular (and unreliable)!

Examples of such techniques:

* Lazy loading of images - Images on the page are not loaded all at once. JavaScript will be used to load an image when the user scrolls into the part of the page that displays the image.
* Prioritizing visible content (or above-the-fold rendering) - Include only the minimum CSS/content/scripts necessary for the amount of page that would be rendered in the users browser first to display as quickly as possible, you can then use deferred scripts or listen for the `DOMContentLoaded`/`load` event to load in other resources and content.
* Async HTML fragments - Flushing parts of the HTML to the browser as the page is constructed on the back end. More details on the technique can be found [here](http://www.ebaytechblog.com/2014/12/08/async-fragments-rediscovering-progressive-html-rendering-with-marko/).

---

### Why you would use a `srcset` attribute in an image tag? Explain the process the browser uses when evaluating the content of this attribute.

TODO

###### References

* https://stackoverflow.com/questions/33651166/what-is-progressive-rendering
* http://www.ebaytechblog.com/2014/12/08/async-fragments-rediscovering-progressive-html-rendering-with-marko/

---

### Have you used different HTML templating languages before?

Yes, Pug (formerly Jade), ERB, Slim, Handlebars, Jinja, Liquid, just to name a few. In my opinion, they are more or less the same and provide similar functionality of escaping content and helpful filters for manipulating the data to be displayed. Most templating engines will also allow you to inject your own filters in the event you need custom processing before display.

### Other Answers

* https://neal.codes/blog/front-end-interview-questions-html/
* http://peterdoes.it/2015/12/03/a-personal-exercise-front-end-job-interview-questions-and-my-answers-all/

---

## CSS Questions

Answers to [Front-end Job Interview Questions - CSS Questions](https://github.com/h5bp/Front-end-Developer-Interview-Questions#css-questions). Pull requests for suggestions and corrections are welcome!

---

### What is CSS selector specificity and how does it work?

The browser determines what styles to show on an element depending on the specificity of CSS rules. We assume that the browser has already determined the rules that match a particular element. Among the matching rules, the specificity, four comma-separate values, `a, b, c, d` are calculated for each rule based on the following:

1. `a` is whether inline styles are being used. If the property declaration is an inline style on the element, `a` is 1, else 0.
2. `b` is the number of ID selectors.
3. `c` is the number of classes, attributes and pseudo-classes selectors.
4. `d` is the number of tags and pseudo-elements selectors.

The resulting specificity is not a score, but a matrix of values that can be compared column by column. When comparing selectors to determine which has the highest specificity, look from left to right, and compare the highest value in each column. So a value in column `b` will override values in columns `c` and `d`, no matter what they might be. As such, specificity of `0,1,0,0` would be greater than one of `0,0,10,10`.

In the cases of equal specificity: the latest rule is the one that counts. If you have written the same rule into your style sheet (regardless of internal or external) twice, then the lower rule in your style sheet is closer to the element to be styled, it is deemed to be more specific and therefore will be applied.

I would write CSS rules with low specificity so that they can be easily overridden if necessary. When writing CSS UI component library code, it is important that they have low specificities so that users of the library can override them without using too complicated CSS rules just for the sake of increasing specificity or resorting to `!important`.

###### References

* https://www.smashingmagazine.com/2007/07/css-specificity-things-you-should-know/
* https://www.sitepoint.com/web-foundations/specificity/

---

### What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why?

* **Resetting** - Resetting is meant to strip all default browser styling on elements. For e.g. `margin`s, `padding`s, `font-size`s of all elements are reset to be the same. You will have to redeclare styling for common typographic elements.
* **Normalizing** - Normalizing preserves useful default styles rather than "unstyling" everything. It also corrects bugs for common browser dependencies.

I would choose resetting when I have a very customized or unconventional site design such that I need to do a lot of my own styling and do not need any default styling to be preserved.

###### References

* https://stackoverflow.com/questions/6887336/what-is-the-difference-between-normalize-css-and-reset-css

---

### Describe `float`s and how they work.

Float is a CSS positioning property. Floated elements remain a part of the flow of the page, and will affect the positioning of other elements (e.g. text will flow around floated elements), unlike `position: absolute` elements, which are removed from the flow of the page.

The CSS `clear` property can be used to be positioned below `left`/`right`/`both` floated elements.

If a parent element contains nothing but floated elements, its height will be collapsed to nothing. It can be fixed by clearing the float after the floated elements in the container but before the close of the container.

The `.clearfix` hack uses a clever CSS pseudo selector (`:after`) to clear floats. Rather than setting the overflow on the parent, you apply an additional class `clearfix` to it. Then apply this CSS:

```css
.clearfix:after {
  content: ' ';
  visibility: hidden;
  display: block;
  height: 0;
  clear: both;
}
```

Alternatively, give `overflow: auto` or `overflow: hidden` property to the parent element which will establish a new block formatting context inside the children and it will expand to contain its children.

###### References

* https://css-tricks.com/all-about-floats/

---

### Describe `z-index` and how stacking context is formed.

The `z-index` property in CSS controls the vertical stacking order of elements that overlap. `z-index` only affects elements that have a `position` value which is not `static`.

Without any `z-index` value, elements stack in the order that they appear in the DOM (the lowest one down at the same hierarchy level appears on top). Elements with non-static positioning (and their children) will always appear on top of elements with default static positioning, regardless of HTML hierarchy.

A stacking context is an element that contains a set of layers. Within a local stacking context, the `z-index` values of its children are set relative to that element rather than to the document root. Layers outside of that context — i.e. sibling elements of a local stacking context — can't sit between layers within it. If an element B sits on top of element A, a child element of element A, element C, can never be higher than element B even if element C has a higher `z-index` than element B.

Each stacking context is self-contained - after the element's contents are stacked, the whole element is considered in the stacking order of the parent stacking context. A handful of CSS properties trigger a new stacking context, such as `opacity` less than 1, `filter` that is not `none`, and `transform` that is not`none`.

###### References

* https://css-tricks.com/almanac/properties/z/z-index/
* https://philipwalton.com/articles/what-no-one-told-you-about-z-index/
* https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Positioning/Understanding_z_index/The_stacking_context

---

### Describe Block Formatting Context (BFC) and how it works.

A Block Formatting Context (BFC) is part of the visual CSS rendering of a web page in which block boxes are laid out. Floats, absolutely positioned elements, `inline-blocks`, `table-cells`, `table-caption`s, and elements with `overflow` other than `visible` (except when that value has been propagated to the viewport) establish new block formatting contexts.

A BFC is an HTML box that satisfies at least one of the following conditions:

* The value of `float` is not `none`.
* The value of `position` is neither `static` nor `relative`.
* The value of `display` is `table-cell`, `table-caption`, `inline-block`, `flex`, or `inline-flex`.
* The value of `overflow` is not `visible`.

In a BFC, each box's left outer edge touches the left edge of the containing block (for right-to-left formatting, right edges touch).

Vertical margins between adjacent block-level boxes in a BFC collapse. Read more on [collapsing margins](https://www.sitepoint.com/web-foundations/collapsing-margins/).

###### References

* https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Block_formatting_context
* https://www.sitepoint.com/understanding-block-formatting-contexts-in-css/

---

### What are the various clearing techniques and which is appropriate for what context?

* Empty `div` method - `<div style="clear:both;"></div>`.
* Clearfix method - Refer to the `.clearfix` class above.
* `overflow: auto` or `overflow: hidden` method - Parent will establish a new block formatting context and expand to contains its floated children.

In large projects, I would write a utility `.clearfix` class and use them in places where I need it. `overflow: hidden` might clip children if the children is taller than the parent and is not very ideal.

---

### Explain CSS sprites, and how you would implement them on a page or site.

CSS sprites combine multiple images into one single larger image. It is commonly used technique for icons (Gmail uses it). How to implement it:

1. Use a sprite generator that packs multiple images into one and generate the appropriate CSS for it.
1. Each image would have a corresponding CSS class with `background-image`, `background-position` and `background-size` properties defined.
1. To use that image, add the corresponding class to your element.

**Advantages:**

* Reduce the number of HTTP requests for multiple images (only one single request is required per spritesheet). But with HTTP2, loading multiple images is no longer much of an issue.
* Advance downloading of assets that won't be downloaded until needed, such as images that only appear upon `:hover` pseudo-states. Blinking wouldn't be seen.

###### References

* https://css-tricks.com/css-sprites/

---

### How would you approach fixing browser-specific styling issues?

* After identifying the issue and the offending browser, use a separate style sheet that only loads when that specific browser is being used. This technique requires server-side rendering though.
* Use libraries like Bootstrap that already handles these styling issues for you.
* Use `autoprefixer` to automatically add vendor prefixes to your code.
* Use Reset CSS or Normalize.css.

---

### How do you serve your pages for feature-constrained browsers? What techniques/processes do you use?

* Graceful degradation - The practice of building an application for modern browsers while ensuring it remains functional in older browsers.
* Progressive enhancement - The practice of building an application for a base level of user experience, but adding functional enhancements when a browser supports it.
* Use [caniuse.com](https://caniuse.com/) to check for feature support.
* Autoprefixer for automatic vendor prefix insertion.
* Feature detection using [Modernizr](https://modernizr.com/).

---

### What are the different ways to visually hide content (and make it available only for screen readers)?

These techniques are related to accessibility (a11y).

* `visibility: hidden`. However the element is still in the flow of the page, and still takes up space.
* `width: 0; height: 0`. Make the element not take up any space on the screen at all, resulting in not showing it.
* `position: absolute; left: -99999px`. Position it outside of the screen.
* `text-indent: -9999px`. This only works on text within the `block` elements.
* Metadata. For example by using Schema.org, RDF and JSON-LD.
* WAI-ARIA. A W3C technical specification that specifies how to increase the accessibility of web pages.

Even if WAI-ARIA is the ideal solution, I would go with the `absolute` positioning approach, as it has the least caveats, works for most elements and it's an easy technique.

###### References

* https://www.w3.org/TR/wai-aria-1.1/
* https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA
* http://a11yproject.com/

---

### Have you ever used a grid system, and if so, what do you prefer?

I like the `float`-based grid system because it still has the most browser support among the alternative existing systems (flex, grid). It has been used in Bootstrap for years and has been proven to work.

---

### Have you used or implemented media queries or mobile-specific layouts/CSS?

Yes. An example would be transforming a stacked pill navigation into a fixed-bottom tab navigation beyond a certain breakpoint.

---

### Are you familiar with styling SVG?

No... Sadly.

---

### Can you give an example of an @media property other than screen?

TODO

---

### What are some of the "gotchas" for writing efficient CSS?

Firstly, understand that browsers match selectors from rightmost (key selector) to left. Browsers filter out elements in the DOM according to the key selector, and traverse up its parent elements to determine matches. The shorter the length of the selector chain, the faster the browser can determine if that element matches the selector. Hence avoid key selectors that are tag and universal selectors. They match a large numbers of elements and browsers will have to do more work in determining if the parents do match.

[BEM (Block Element Modifier)](https://bem.info/) methodology recommends that everything has a single class, and, where you need hierarchy, that gets baked into the name of the class as well, this naturally makes the selector efficient and easy to override.

Be aware of which CSS properties trigger reflow, repaint and compositing. Avoid writing styles that change the layout (trigger reflow) where possible.

###### References

* https://developers.google.com/web/fundamentals/performance/rendering/
* https://csstriggers.com/

---

### What are the advantages/disadvantages of using CSS preprocessors?

**Advantages:**

* CSS is made more maintainable.
* Easy to write nested selectors.
* Variables for consistent theming. Can share theme files across different projects.
* Mixins to generate repeated CSS.
* Splitting your code into multiple files. CSS files can be split up too but doing so will require a HTTP request to download each CSS file.

**Disadvantages:**

* Requires tools for preprocessing. Re-compilation time can be slow.

---

### Describe what you like and dislike about the CSS preprocessors you have used.

**Likes:**

* Mostly the advantages mentioned above.
* Less is written in JavaScript, which plays well with Node.

**Dislikes:**

* I use Sass via `node-sass`, which is a binding for LibSass written in C++. I have to frequently recompile it when switching between node versions.
* In Less, variable names are prefixed with `@`, which can be confused with native CSS keywords like `@media`, `@import` and `@font-face` rule.

---

### How would you implement a web design comp that uses non-standard fonts?

Use `@font-face` and define `font-family` for different `font-weight`s.

---

### Explain how a browser determines what elements match a CSS selector.

This part is related to the above about writing efficient CSS. Browsers match selectors from rightmost (key selector) to left. Browsers filter out elements in the DOM according to the key selector, and traverse up its parent elements to determine matches. The shorter the length of the selector chain, the faster the browser can determine if that element matches the selector.

For example with this selector `p span`, browsers firstly find all the `<span>` elements, and traverse up its parent all the way up to the root to find the `<p>` element. For a particular `<span>`, as soon as it finds a `<p>`, it knows that the `<span>` matches and can stop its matching.

###### References

* https://stackoverflow.com/questions/5797014/why-do-browsers-match-css-selectors-from-right-to-left

---

### Describe pseudo-elements and discuss what they are used for.

A CSS pseudo-element is a keyword added to a selector that lets you style a specific part of the selected element(s). They can be used for decoration (`:first-line`, `:first-letter`) or adding elements to the markup (combined with `content: ...`) without having to modify the markup (`:before`, `:after`).

* `:first-line` and `:first-letter` can be used to decorate text.
* Used in the `.clearfix` hack as shown above to add a zero-space element with `clear: both`.
* Triangular arrows in tooltips use `:before` and `:after`. Encourages separation of concerns because the triangle is considered part of styling and not really the DOM. It's not really possible to draw a triangle with just CSS styles without using an additional HTML element.

###### References

* https://css-tricks.com/almanac/selectors/a/after-and-before/

---

### Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.

The CSS box model describes the rectangular boxes that are generated for elements in the document tree and laid out according to the visual formatting model. Each box has a content area (e.g. text, an image, etc.) and optional surrounding `padding`, `border`, and `margin` areas.

The CSS box model is responsible for calculating:

* How much space a block element takes up.
* Whether or not borders and/or margins overlap, or collapse.
* A box's dimensions.

The box model has the following rules:

* The dimensions of a block element are calculated by `width`, `height`, `padding`, `border`s, and `margin`s.
* If no `height` is specified, a block element will be as high as the content it contains, plus `padding` (unless there are floats, for which see below).
* If no `width` is specified, a non-floated block element will expand to fit the width of its parent minus `padding`.
* The `height` of an element is calculated by the content's `height`.
* The `width` of an element is calculated by the content's `width`.
* By default, `padding`s and `border`s are not part of the `width` and `height` of an element.

###### References

* https://www.smashingmagazine.com/2010/06/the-principles-of-cross-browser-css-coding/#understand-the-css-box-model

---

### What does `* { box-sizing: border-box; }` do? What are its advantages?

* By default, elements have `box-sizing: content-box` applied, and only the content size is being accounted for.
* `box-sizing: border-box` changes how the `width` and `height` of elements are being calculated, `border` and `padding` are also being included in the calculation.
* The `height` of an element is now calculated by the content's `height` + vertical `padding` + vertical `border` width.
* The `width` of an element is now calculated by the content's `width` + horizontal `padding` + horizontal `border` width.

---

### What is the CSS `display` property and can you give a few examples of its use?

* `none`, `block`, `inline`, `inline-block`, `table`, `table-row`, `table-cell`, `list-item`.

TODO

---

### What's the difference between `inline` and `inline-block`?

I shall throw in a comparison with `block` for good measure.

|                                      | `block`                                                                                     | `inline-block`                                                   | `inline`                                                                                                                                                                                                             |
| ------------------------------------ | ------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Size                                 | Fills up the width of its parent container.                                                 | Depends on content.                                              | Depends on content.                                                                                                                                                                                                  |
| Positioning                          | Start on a new line and tolerates no HTML elements next to it (except when you add `float`) | Flows along with other content and allows other elements beside. | Flows along with other content and allows other elements beside.                                                                                                                                                     |
| Can specify `width` and `height`     | Yes                                                                                         | Yes                                                              | No. Will ignore if being set.                                                                                                                                                                                        |
| Can be aligned with `vertical-align` | No                                                                                          | Yes                                                              | Yes                                                                                                                                                                                                                  |
| Margins and paddings                 | All sides respected.                                                                        | All sides respected.                                             | Only horizontal sides respected. Vertical sides, if specified, do not affect layout. Vertical space it takes up depends on `line-height`, even though the `border` and `padding` appear visually around the content. |
| Float                                | -                                                                                           | -                                                                | Becomes like a `block` element where you can set vertical margins and paddings.                                                                                                                                      |

---

### What's the difference between a `relative`, `fixed`, `absolute` and `static`ally positioned element?

A positioned element is an element whose computed `position` property is either `relative`, `absolute`, `fixed` or `sticky`.

* `static` - The default position; the element will flow into the page as it normally would. The `top`, `right`, `bottom`, `left` and `z-index` properties do not apply.
* `relative` - The element's position is adjusted relative to itself, without changing layout (and thus leaving a gap for the element where it would have been had it not been positioned).
* `absolute` - The element is removed from the flow of the page and positioned at a specified position relative to its closest positioned ancestor if any, or otherwise relative to the initial containing block. Absolutely positioned boxes can have margins, and they do not collapse with any other margins. These elements do not affect the position of other elements.
* `fixed` - The element is removed from the flow of the page and positioned at a specified position relative to the viewport and doesn't move when scrolled.
* `sticky` - Sticky positioning is a hybrid of relative and fixed positioning. The element is treated as `relative` positioned until it crosses a specified threshold, at which point it is treated as `fixed` positioned.

###### References

* https://developer.mozilla.org/en/docs/Web/CSS/position

---

### What existing CSS frameworks have you used locally, or in production? How would you change/improve them?

* **Bootstrap** - Slow release cycle. Bootstrap 4 has been in alpha for almost 2 years. Add a spinner button component, as it is widely-used.
* **Semantic UI** - Source code structure makes theme customization extremely hard to understand. Painful to customize with unconventional theming system. Hardcoded config path within the vendor library. Not well-designed for overriding variables unlike in Bootstrap.
* **Bulma** - A lot of non-semantic and superfluous classes and markup required. Not backward compatible. Upgrading versions breaks the app in subtle manners.

---

### Have you played around with the new CSS Flexbox or Grid specs?

Yes. Flexbox is mainly meant for 1-dimensional layouts while Grid is meant for 2-dimensional layouts.

Flexbox solves many common problems in CSS, such as vertical centering of elements within a container, sticky footer, etc. Bootstrap and Bulma are based on Flexbox, and it is probably the recommended way to create layouts these days. Have tried Flexbox before but ran into some browser incompatibility issues (Safari) in using `flex-grow`, and I had to rewrite my code using `inline-blocks` and math to calculate the widths in percentages, it wasn't a nice experience.

Grid is by far the most intuitive approach for creating grid-based layouts (it better be!) but browser support is not wide at the moment.

###### References

* https://philipwalton.github.io/solved-by-flexbox/

---

### Can you explain the difference between coding a web site to be responsive versus using a mobile-first strategy?

TODO

---

### How is responsive design different from adaptive design?

Both responsive and adaptive design attempt to optimize the user experience across different devices, adjusting for different viewport sizes, resolutions, usage contexts, control mechanisms, and so on.

Responsive design works on the principle of flexibility - a single fluid website that can look good on any device. Responsive websites use media queries, flexible grids, and responsive images to create a user experience that flexes and changes based on a multitude of factors. Like a single ball growing or shrinking to fit through several different hoops.

Adaptive design is more like the modern definition of progressive enhancement. Instead of one flexible design, adaptive design detects the device and other features, and then provides the appropriate feature and layout based on a predefined set of viewport sizes and other characteristics. The site detects the type of device used, and delivers the pre-set layout for that device. Instead of a single ball going through several different-sized hoops, you'd have several different balls to use depending on the hoop size.

###### References

* https://developer.mozilla.org/en-US/docs/Archive/Apps/Design/UI_layout_basics/Responsive_design_versus_adaptive_design
* http://mediumwell.com/responsive-adaptive-mobile/
* https://css-tricks.com/the-difference-between-responsive-and-adaptive-design/

---

### Have you ever worked with retina graphics? If so, when and what techniques did you use?

I tend to use higher resolution graphics (twice the display size) to handle retina display. The better way would be to use a media query like `@media only screen and (min-device-pixel-ratio: 2) { ... }` and change the `background-image`.

For icons, I would also opt to use svgs and icon fonts where possible, as they render very crisply regardless of resolution.

Another method would be to use JavaScript to replace the `<img>` `src` attribute with higher resolution versions after checking the `window.devicePixelRatio` value.

###### References

* https://www.sitepoint.com/css-techniques-for-retina-displays/

---

### Is there any reason you'd want to use `translate()` instead of `absolute` positioning, or vice-versa? And why?

`translate()` is a value of CSS `transform`. Changing `transform` or `opacity` does not trigger browser reflow or repaint, only compositions, whereas changing the absolute positioning triggers `reflow`. `transform` causes the browser to create a GPU layer for the element but changing absolute positioning properties uses the CPU. Hence `translate()` is more efficient and will result in shorter paint times for smoother animations.

When using `translate()`, the element still takes up its original space (sort of like `position: relative`), unlike in changing the absolute positioning.

###### References

* https://www.paulirish.com/2012/why-moving-elements-with-translate-is-better-than-posabs-topleft/

---

### Other Answers

* https://neal.codes/blog/front-end-interview-css-questions
* https://quizlet.com/28293152/front-end-interview-questions-css-flash-cards/
* http://peterdoes.it/2015/12/03/a-personal-exercise-front-end-job-interview-questions-and-my-answers-all/

---

## JS Questions

Answers to [Front-end Job Interview Questions - JS Questions](https://github.com/h5bp/Front-end-Developer-Interview-Questions#js-questions). Pull requests for suggestions and corrections are welcome!

---

### Explain event delegation

Event delegation is a technique involving adding event listeners to a parent element instead of adding them to the descendant elements. The listener will fire whenever the event is triggered on the descendant elements due to event bubbling up the DOM. The benefits of this technique are:

* Memory footprint goes down because only one single handler is needed on the parent element, rather than having to attach event handlers on each descendant.
* There is no need to unbind the handler from elements that are removed and to bind the event for new elements.

###### References

* https://davidwalsh.name/event-delegate
* https://stackoverflow.com/questions/1687296/what-is-dom-event-delegation

---

### Explain how `this` works in JavaScript

There's no simple explanation for `this`; it is one of the most confusing concepts in JavaScript. A hand-wavey explanation is that the value of `this` depends on how the function is called. I have read many explanations on `this` online, and I found [Arnav Aggrawal](https://medium.com/@arnav_aggarwal)'s explanation to be the clearest. The following rules are applied:

1. If the `new` keyword is used when calling the function, `this` inside the function is a brand new object.
2. If `apply`, `call`, or `bind` are used to call/create a function, `this` inside the function is the object that is passed in as the argument.
3. If a function is called as a method, such as `obj.method()` — `this` is the object that the function is a property of.
4. If a function is invoked as a free function invocation, meaning it was invoked without any of the conditions present above, `this` is the global object. In a browser, it is the `window` object. If in strict mode (`'use strict'`), `this` will be `undefined` instead of the global object.
5. If multiple of the above rules apply, the rule that is higher wins and will set the `this` value.
6. If the function is an ES2015 arrow function, it ignores all the rules above and receives the `this` value of its surrounding scope at the time it is created.

For an in-depth explanation, do check out his [article on Medium](https://codeburst.io/the-simple-rules-to-this-in-javascript-35d97f31bde3).

###### References

* https://codeburst.io/the-simple-rules-to-this-in-javascript-35d97f31bde3
* https://stackoverflow.com/a/3127440/1751946

---

### Explain how prototypal inheritance works

This is an extremely common JavaScript interview question. All JavaScript objects have a `prototype` property, that is a reference to another object. When a property is accessed on an object and if the property is not found on that object, the JavaScript engine looks at the object's `prototype`, and the `prototype`'s `prototype` and so on, until it finds the property defined on one of the `prototype`s or until it reaches the end of the prototype chain. This behaviour simulates classical inheritance, but it is really more of [delegation than inheritance](https://davidwalsh.name/javascript-objects).

###### References

* https://www.quora.com/What-is-prototypal-inheritance/answer/Kyle-Simpson
* https://davidwalsh.name/javascript-objects

---

### What do you think of AMD vs CommonJS?

Both are ways to implement a module system, which was not natively present in JavaScript until ES2015 came along. CommonJS is synchronous while AMD (Asynchronous Module Definition) is obviously asynchronous. CommonJS is designed with server-side development in mind while AMD, with its support for asynchronous loading of modules, is more intended for browsers.

I find AMD syntax to be quite verbose and CommonJS is closer to the style you would write import statements in other languages. Most of the time, I find AMD unnecessary, because if you served all your JavaScript into one concatenated bundle file, you wouldn't benefit from the async loading properties. Also, CommonJS syntax is closer to Node style of writing modules and there is less context-switching overhead when switching between client side and server side JavaScript development.

I'm glad that with ES2015 modules, that has support for both synchronous and asynchronous loading, we can finally just stick to one approach. Although it hasn't been fully rolled out in browsers and in Node, we can always use transpilers to convert our code.

###### References

* https://auth0.com/blog/javascript-module-systems-showdown/
* https://stackoverflow.com/questions/16521471/relation-between-commonjs-amd-and-requirejs

---

### Explain why the following doesn't work as an IIFE: `function foo(){ }();`. What needs to be changed to properly make it an IIFE?

IIFE stands for Immediately Invoked Function Expressions. The JavaScript parser reads `function foo(){ }();` as `function foo(){ }` and `();`, where the former is a function declaration and the latter (a pair of brackets) is an attempt at calling a function but there is no name specified, hence it throws `Uncaught SyntaxError: Unexpected token )`.

Here are two ways to fix it that involves adding more brackets: `(function foo(){ })()` and `(function foo(){ }())`. These functions are not exposed in the global scope and you can even omit its name if you do not need to reference itself within the body.

###### References

* http://lucybain.com/blog/2014/immediately-invoked-function-expression/

---

### What's the difference between a variable that is: `null`, `undefined` or undeclared? How would you go about checking for any of these states?

**Undeclared** variables are created when you assign to a value to an identifier that is not previously created using `var`, `let` or `const`. Undeclared variables will be defined globally, outside of the current scope. In strict mode, a `ReferenceError` will be thrown when you try to assign to an undeclared variable. Undeclared variables are bad just like how global variables are bad. Avoid them at all cost! To check for them, wrap its usage in a `try`/`catch` block.

```js
function foo() {
  x = 1; // Throws a ReferenceError in strict mode
}

foo();
console.log(x); // 1
```

A variable that is `undefined` is a variable that has been declared, but not assigned a value. It is of type `undefined`. If a function does not return any value as the result of executing it is assigned to a variable, the variable also has the value of `undefined`. To check for it, compare using the strict equality (`===`) operator or `typeof` which will give the `'undefined'` string. Note that you should not be using the abstract equality operator to check, as it will also return `true` if the value is `null`.

```js
var foo;
console.log(foo); // undefined
console.log(foo === undefined); // true
console.log(typeof foo === 'undefined'); // true

console.log(foo == null); // true. Wrong, don't use this to check!

function bar() {}
var baz = bar();
console.log(baz); // undefined
```

A variable that is `null` will have been explicitly assigned to the `null` value. It represents no value and is different from `undefined` in the sense that it has been explicitly assigned. To check for `null,` simply compare using the strict equality operator. Note that like the above, you should not be using the abstract equality operator (`==`) to check, as it will also return `true` if the value is `undefined`.

```js
var foo = null;
console.log(foo === null); // true

console.log(foo == undefined); // true. Wrong, don't use this to check!
```

As a personal habit, I never leave my variables undeclared or unassigned. I will explicitly assign `null` to them after declaring, if I don't intend to use it yet.

###### References

* https://stackoverflow.com/questions/15985875/effect-of-declared-and-undeclared-variables
* https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/undefined

---

### What is a closure, and how/why would you use one?

A closure is the combination of a function and the lexical environment within which that function was declared. The word "lexical" refers to the fact that lexical scoping uses the location where a variable is declared within the source code to determine where that variable is available. Closures are functions that have access to the outer (enclosing) function's variables—scope chain even after the outer function has returned.

**Why would you use one?**

* Data privacy / emulating private methods with closures. Commonly used in the [module pattern](https://addyosmani.com/resources/essentialjsdesignpatterns/book/#modulepatternjavascript).
* [Partial applications or currying](https://medium.com/javascript-scene/curry-or-partial-application-8150044c78b8#.l4b6l1i3x).

###### References

* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures
* https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-closure-b2f0d2152b36

---

### Can you describe the main difference between a `.forEach` loop and a `.map()` loop and why you would pick one versus the other?

To understand the differences between the two, let's look at what each function does.

**`forEach`**

* Iterates through the elements in an array.
* Executes a callback for each element.
* Does not return a value.

```js
const a = [1, 2, 3];
const doubled = a.forEach((num, index) => {
  // Do something with num and/or index.
});

// doubled = undefined
```

**`map`**

* Iterates through the elements in an array.
* "Maps" each element to a new element by calling the function on each element, creating a new array as a result.

```js
const a = [1, 2, 3];
const doubled = a.map(num => {
  return num * 2;
});

// doubled = [2, 4, 6]
```

The main difference between `.forEach` and `.map()` is that `.map()` returns a new array. If you need the result, but do not wish to mutate the original array, `.map()` is the clear choice. If you simply need to iterate over an array, `forEach` is a fine choice.

###### References

* https://codeburst.io/javascript-map-vs-foreach-f38111822c0f

---

### What's a typical use case for anonymous functions?

They can be used in IIFEs to encapsulate some code within a local scope so that variables declared in it do not leak to the global scope.

```js
(function() {
  // Some code here.
})();
```

As a callback that is used once and does not need to be used anywhere else. The code will seem more self-contained and readable when handlers are defined right inside the code calling them, rather than having to search elsewhere to find the function body.

```js
setTimeout(function() {
  console.log('Hello world!');
}, 1000);
```

Arguments to functional programming constructs or Lodash (similar to callbacks).

```js
const arr = [1, 2, 3];
const double = arr.map(function(el) {
  return el * 2;
});
console.log(double); // [2, 4, 6]
```

###### References

* https://www.quora.com/What-is-a-typical-usecase-for-anonymous-functions
* https://stackoverflow.com/questions/10273185/what-are-the-benefits-to-using-anonymous-functions-instead-of-named-functions-fo

---

### How do you organize your code? (module pattern, classical inheritance?)

In the past, I used Backbone for my models which encourages a more OOP approach, creating Backbone models and attaching methods to them.

The module pattern is still great, but these days, I use the Flux architecture based on React/Redux which encourages a single-directional functional programming approach instead. I would represent my app's models using plain objects and write utility pure functions to manipulate these objects. State is manipulated using actions and reducers like in any other Redux application.

I avoid using classical inheritance where possible. When and if I do, I stick to [these rules](https://medium.com/@dan_abramov/how-to-use-classes-and-sleep-at-night-9af8de78ccb4).

---

### What's the difference between host objects and native objects?

Native objects are objects that are part of the JavaScript language defined by the ECMAScript specification, such as `String`, `Math`, `RegExp`, `Object`, `Function`, etc.

Host objects are provided by the runtime environment (browser or Node), such as `window`, `XMLHTTPRequest`, etc.

###### References

* https://stackoverflow.com/questions/7614317/what-is-the-difference-between-native-objects-and-host-objects

---

### Difference between: `function Person(){}`, `var person = Person()`, and `var person = new Person()`?

This question is pretty vague. My best guess at its intention is that it is asking about constructors in JavaScript. Technically speaking, `function Person(){}` is just a normal function declaration. The convention is use PascalCase for functions that are intended to be used as constructors.

`var person = Person()` invokes the `Person` as a function, and not as a constructor. Invoking as such is a common mistake if it the function is intended to be used as a constructor. Typically, the constructor does not return anything, hence invoking the constructor like a normal function will return `undefined` and that gets assigned to the variable intended as the instance.

`var person = new Person()` creates an instance of the `Person` object using the `new` operator, which inherits from `Person.prototype`. An alternative would be to use `Object.create`, such as: `Object.create(Person.prototype)`.

```js
function Person(name) {
  this.name = name;
}

var person = Person('John');
console.log(person); // undefined
console.log(person.name); // Uncaught TypeError: Cannot read property 'name' of undefined

var person = new Person('John');
console.log(person); // Person { name: "John" }
console.log(person.name); // "john"
```

###### References

* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/new

---

### What's the difference between `.call` and `.apply`?

Both `.call` and `.apply` are used to invoke functions and the first parameter will be used as the value of `this` within the function. However, `.call` takes in a comma-separated arguments as the next arguments while `.apply` takes in an array of arguments as the next argument. An easy way to remember this is C for `call` and comma-separated and A for `apply` and array of arguments.

```js
function add(a, b) {
  return a + b;
}

console.log(add.call(null, 1, 2)); // 3
console.log(add.apply(null, [1, 2])); // 3
```

---

### Explain `Function.prototype.bind`.

Taken word-for-word from [MDN](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_objects/Function/bind):

> The `bind()` method creates a new function that, when called, has its this keyword set to the provided value, with a given sequence of arguments preceding any provided when the new function is called.

In my experience, it is most useful for binding the value of `this` in methods of classes that you want to pass into other functions. This is frequently done in React components.

###### References

* https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_objects/Function/bind

---

### When would you use `document.write()`?

`document.write()` writes a string of text to a document stream opened by `document.open()`. When `document.write()` is executed after the page has loaded, it will call `document.open` which clears the whole document (`<head>` and `<body>` removed!) and replaces the contents with the given parameter value in string. Hence it is usually considered dangerous and prone to misuse.

There are some answers online that explain `document.write()` is being used in analytics code or [when you want to include styles that should only work if JavaScript is enabled](https://www.quirksmode.org/blog/archives/2005/06/three_javascrip_1.html). It is even being used in HTML5 boilerplate to [load scripts in parallel and preserve execution order](https://github.com/paulirish/html5-boilerplate/wiki/Script-Loading-Techniques#documentwrite-script-tag)! However, I suspect those reasons might be outdated and in the modern day, they can be achieved without using `document.write()`. Please do correct me if I'm wrong about this.

###### References

* https://www.quirksmode.org/blog/archives/2005/06/three_javascrip_1.html
* https://github.com/h5bp/html5-boilerplate/wiki/Script-Loading-Techniques#documentwrite-script-tag

---

### What's the difference between feature detection, feature inference, and using the UA string?

**Feature Detection**

Feature detection involves working out whether a browser supports a certain block of code, and running different code dependent on whether it does (or doesn't), so that the browser can always provide a working experience rather crashing/erroring in some browsers. For example:

```js
if ('geolocation' in navigator) {
  // Can use navigator.geolocation
} else {
  // Handle lack of feature
}
```

[Modernizr](https://modernizr.com/) is a great library to handle feature detection.

**Feature Inference**

Feature inference checks for a feature just like feature detection, but uses another function because it assumes it will also exist, e.g.:

```js
if (document.getElementsByTagName) {
  element = document.getElementById(id);
}
```

This is not really recommended. Feature detection is more foolproof.

**UA String**

This is a browser-reported string that allows the network protocol peers to identify the application type, operating system, software vendor or software version of the requesting software user agent. It can be accessed via `navigator.userAgent`. However, the string is tricky to parse and can be spoofed. For example, Chrome reports both as Chrome and Safari. So to detect Safari you have to check for the Safari string and the absence of the Chrome string. Avoid this method.

###### References

* https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Cross_browser_testing/Feature_detection
* https://stackoverflow.com/questions/20104930/whats-the-difference-between-feature-detection-feature-inference-and-using-th
* https://developer.mozilla.org/en-US/docs/Web/HTTP/Browser_detection_using_the_user_agent

---

### Explain Ajax in as much detail as possible.

Ajax (asynchronous JavaScript and XML) is a set of web development techniques using many web technologies on the client side to create asynchronous web applications. With Ajax, web applications can send data to and retrieve from a server asynchronously (in the background) without interfering with the display and behavior of the existing page. By decoupling the data interchange layer from the presentation layer, Ajax allows for web pages, and by extension web applications, to change content dynamically without the need to reload the entire page. In practice, modern implementations commonly substitute JSON for XML due to the advantages of being native to JavaScript.

The `XMLHttpRequest` API is frequently used for the asynchronous communication or these days, the `fetch` API.

###### References

* https://en.wikipedia.org/wiki/Ajax_(programming)
* https://developer.mozilla.org/en-US/docs/AJAX

---

### What are the advantages and disadvantages of using Ajax?

**Advantages**

* Better interactivity. New content from the server can be changed dynamically without the need to reload the entire page.
* Reduce connections to the server since scripts and stylesheets only have to be requested once.
* State can be maintained on a page. JavaScript variables and DOM state will persist because the main container page was not reloaded.
* Basically most of the advantages of an SPA.

**Disadvantages**

* Dynamic webpages are harder to bookmark.
* Does not work if JavaScript has been disabled in the browser.
* Some webcrawlers do not execute JavaScript and would not see content that has been loaded by JavaScript.
* Basically most of the disadvantages of an SPA.

---

### Explain how JSONP works (and how it's not really Ajax).

JSONP (JSON with Padding) is a method commonly used to bypass the cross-domain policies in web browsers because Ajax requests from the current page to a cross-origin domain is not allowed.

JSONP works by making a request to a cross-origin domain via a `<script>` tag and usually with a `callback` query parameter, for example: `https://example.com?callback=printData`. The server will then wrap the data within a function called `printData` and return it to the client.

```html
<!-- https://mydomain.com -->
<script>
function printData(data) {
  console.log(`My name is ${data.name}!`);
}
</script>

<script src="https://example.com?callback=printData"></script>
```

```js
// File loaded from https://example.com?callback=printData
printData({ name: 'Yang Shun' });
```

The client has to have the `printData` function in its global scope and the function will be executed by the client when the response from the cross-origin domain is received.

JSONP can be unsafe and has some security implications. As JSONP is really JavaScript, it can do everything else JavaScript can do, so you need to trust the provider of the JSONP data.

These days, [CORS](http://en.wikipedia.org/wiki/Cross-origin_resource_sharing) is the recommended approach and JSONP is seen as a hack.

###### References

* https://stackoverflow.com/a/2067584/1751946

---

### Have you ever used JavaScript templating? If so, what libraries have you used?

Yes. Handlebars, Underscore, Lodash, AngularJS and JSX. I disliked templating in AngularJS because it made heavy use of strings in the directives and typos would go uncaught. JSX is my new favourite as it is closer to JavaScript and there is barely any syntax to learn. Nowadays, you can even use ES2015 template string literals as a quick way for creating templates without relying on third-party code.

```js
const template = `<div>My name is: ${name}</div>`;
```

However, do be aware of a potential XSS in the above approach as the contents are not escaped for you, unlike in templating libraries.

---

### Explain "hoisting".

Hoisting is a term used to explain the behavior of variable declarations in your code. Variables declared or initialized with the `var` keyword will have their declaration "hoisted" up to the top of the current scope. However, only the declaration is hoisted, the assignment (if there is one), will stay where it is. Let's explain with a few examples.

```js
// var declarations are hoisted.
console.log(foo); // undefined
var foo = 1;
console.log(foo); // 1

// let/const declarations are NOT hoisted.
console.log(bar); // ReferenceError: bar is not defined
let bar = 2;
console.log(bar); // 2
```

Function declarations have the body hoisted while the function expressions (written in the form of variable declarations) only has the variable declaration hoisted.

```js
// Function Declaration
console.log(foo); // [Function: foo]
foo(); // 'FOOOOO'
function foo() {
  console.log('FOOOOO');
}
console.log(foo); // [Function: foo]

// Function Expression
console.log(bar); // undefined
bar(); // Uncaught TypeError: bar is not a function
var bar = function() {
  console.log('BARRRR');
};
console.log(bar); // [Function: bar]
```

---

### Describe event bubbling.

When an event triggers on a DOM element, it will attempt to handle the event if there is a listener attached, then the event is bubbled up to its parent and the same thing happens. This bubbling occurs up the element's ancestors all the way to the `document`. Event bubbling is the mechanism behind event delegation.

---

### What's the difference between an "attribute" and a "property"?

Attributes are defined on the HTML markup but properties are defined on the DOM. To illustrate the difference, imagine we have this text field in our HTML: `<input type="text" value="Hello">`.

```js
const input = document.querySelector('input');
console.log(input.getAttribute('value')); // Hello
console.log(input.value); // Hello
```

But after you change the value of the text field by adding "World!" to it, this becomes:

```js
console.log(input.getAttribute('value')); // Hello
console.log(input.value); // Hello World!
```

###### References

* https://stackoverflow.com/questions/6003819/properties-and-attributes-in-html

---

### Why is extending built-in JavaScript objects not a good idea?

Extending a built-in/native JavaScript object means adding properties/functions to its `prototype`. While this may seem like a good idea at first, it is dangerous in practice. Imagine your code uses a few libraries that both extend the `Array.prototype` by adding the same `contains` method, the implementations will overwrite each other and your code will break if the behavior of these two methods are not the same.

The only time you may want to extend a native object is when you want to create a polyfill, essentially providing your own implementation for a method that is part of the JavaScript specification but might not exist in the user's browser due to it being an older browser.

###### References

* http://lucybain.com/blog/2014/js-extending-built-in-objects/

---

### Difference between document `load` event and document `DOMContentLoaded` event?

The `DOMContentLoaded` event is fired when the initial HTML document has been completely loaded and parsed, without waiting for stylesheets, images, and subframes to finish loading.

`window`'s `load` event is only fired after the DOM and all dependent resources and assets have loaded.

###### References

* https://developer.mozilla.org/en-US/docs/Web/Events/DOMContentLoaded
* https://developer.mozilla.org/en-US/docs/Web/Events/load

---

### What is the difference between `==` and `===`?

`==` is the abstract equality operator while `===` is the strict equality operator. The `==` operator will compare for equality after doing any necessary type conversions. The `===` operator will not do type conversion, so if two values are not the same type `===` will simply return `false`. When using `==`, funky things can happen, such as:

```js
1 == '1'; // true
1 == [1]; // true
1 == true; // true
0 == ''; // true
0 == '0'; // true
0 == false; // true
```

My advice is never to use the `==` operator, except for convenience when comparing against `null` or `undefined`, where `a == null` will return `true` if `a` is `null` or `undefined`.

```js
var a = null;
console.log(a == null); // true
console.log(a == undefined); // true
```

###### References

* https://stackoverflow.com/questions/359494/which-equals-operator-vs-should-be-used-in-javascript-comparisons

---

### Explain the same-origin policy with regards to JavaScript.

The same-origin policy prevents JavaScript from making requests across domain boundaries. An origin is defined as a combination of URI scheme, hostname, and port number. This policy prevents a malicious script on one page from obtaining access to sensitive data on another web page through that page's Document Object Model.

###### References

* https://en.wikipedia.org/wiki/Same-origin_policy

---

### Make this work:

```js
duplicate([1, 2, 3, 4, 5]); // [1,2,3,4,5,1,2,3,4,5]
```

```js
function duplicate(arr) {
  return arr.concat(arr);
}

duplicate([1, 2, 3, 4, 5]); // [1,2,3,4,5,1,2,3,4,5]
```

---

### Why is it called a Ternary expression, what does the word "Ternary" indicate?

"Ternary" indicates three, and a ternary expression accepts three operands, the test condition, the "then" expression and the "else" expression. Ternary expressions are not specific to JavaScript and I'm not sure why it is even in this list.

###### References

* https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Operators/Conditional_Operator

---

### What is `"use strict";`? What are the advantages and disadvantages to using it?

'use strict' is a statement used to enable strict mode to entire scripts or individual functions. Strict mode is a way to opt in to a restricted variant of JavaScript.

Advantages:

* Makes it impossible to accidentally create global variables.
* Makes assignments which would otherwise silently fail to throw an exception.
* Makes attempts to delete undeletable properties throw (where before the attempt would simply have no effect).
* Requires that function parameter names be unique.
* `this` is undefined in the global context.
* It catches some common coding bloopers, throwing exceptions.
* It disables features that are confusing or poorly thought out.

Disadvantages:

* Many missing features that some developers might be used to.
* No more access to `function.caller` and `function.arguments`.
* Concatenation of scripts written in different strict modes might cause issues.

Overall, I think the benefits outweigh the disadvantages, and I never had to rely on the features that strict mode blocks. I would recommend using strict mode.

###### References

* http://2ality.com/2011/10/strict-mode-hatred.html
* http://lucybain.com/blog/2014/js-use-strict/

---

### Create a for loop that iterates up to `100` while outputting **"fizz"** at multiples of `3`, **"buzz"** at multiples of `5` and **"fizzbuzz"** at multiples of `3` and `5`.

Check out this version of FizzBuzz by [Paul Irish](https://gist.github.com/jaysonrowe/1592432#gistcomment-790724).

```js
for (let i = 1; i <= 100; i++) {
  let f = i % 3 == 0,
    b = i % 5 == 0;
  console.log(f ? (b ? 'FizzBuzz' : 'Fizz') : b ? 'Buzz' : i);
}
```

I would not advise you to write the above during interviews though. Just stick with the long but clear approach. For more wacky versions of FizzBuzz, check out the reference link below.

###### References

* https://gist.github.com/jaysonrowe/1592432

---

### Why is it, in general, a good idea to leave the global scope of a website as-is and never touch it?

Every script has access to the global scope, and if everyone is using the global namespace to define their own variables, there will bound to be collisions. Use the module pattern (IIFEs) to encapsulate your variables within a local namespace.

---

### Why would you use something like the `load` event? Does this event have disadvantages? Do you know any alternatives, and why would you use those?

The `load` event fires at the end of the document loading process. At this point, all of the objects in the document are in the DOM, and all the images, scripts, links and sub-frames have finished loading.

The DOM event `DOMContentLoaded` will fire after the DOM for the page has been constructed, but do not wait for other resources to finish loading. This is preferred in certain cases when you do not need the full page to be loaded before initializing.

TODO.

###### References

* https://developer.mozilla.org/en-US/docs/Web/API/GlobalEventHandlers/onload

---

### Explain what a single page app is and how to make one SEO-friendly.

The below is taken from the awesome [Grab Front End Guide](https://github.com/grab/front-end-guide), which coincidentally, is written by me!

Web developers these days refer to the products they build as web apps, rather than websites. While there is no strict difference between the two terms, web apps tend to be highly interactive and dynamic, allowing the user to perform actions and receive a response for their action. Traditionally, the browser receives HTML from the server and renders it. When the user navigates to another URL, a full-page refresh is required and the server sends fresh new HTML for the new page. This is called server-side rendering.

However in modern SPAs, client-side rendering is used instead. The browser loads the initial page from the server, along with the scripts (frameworks, libraries, app code) and stylesheets required for the whole app. When the user navigates to other pages, a page refresh is not triggered. The URL of the page is updated via the [HTML5 History API](https://developer.mozilla.org/en-US/docs/Web/API/History_API). New data required for the new page, usually in JSON format, is retrieved by the browser via [AJAX](https://developer.mozilla.org/en-US/docs/AJAX/Getting_Started) requests to the server. The SPA then dynamically updates the page with the data via JavaScript, which it has already downloaded in the initial page load. This model is similar to how native mobile apps work.

The benefits:

* The app feels more responsive and users do not see the flash between page navigations due to full-page refreshes.
* Fewer HTTP requests are made to the server, as the same assets do not have to be downloaded again for each page load.
* Clear separation of the concerns between the client and the server; you can easily build new clients for different platforms (e.g. mobile, chatbots, smart watches) without having to modify the server code. You can also modify the technology stack on the client and server independently, as long as the API contract is not broken.

The downsides:

* Heavier initial page load due to loading of framework, app code, and assets required for multiple pages.
* There's an additional step to be done on your server which is to configure it to route all requests to a single entry point and allow client-side routing to take over from there.
* SPAs are reliant on JavaScript to render content, but not all search engines execute JavaScript during crawling, and they may see empty content on your page. This inadvertently hurts the Search Engine Optimization (SEO) of your app. However, most of the time, when you are building apps, SEO is not the most important factor, as not all the content needs to be indexable by search engines. To overcome this, you can either server-side render your app or use services such as [Prerender](https://prerender.io/) to "render your javascript in a browser, save the static HTML, and return that to the crawlers".

###### References

* https://github.com/grab/front-end-guide#single-page-apps-spas
* http://stackoverflow.com/questions/21862054/single-page-app-advantages-and-disadvantages
* http://blog.isquaredsoftware.com/presentations/2016-10-revolution-of-web-dev/
* https://medium.freecodecamp.com/heres-why-client-side-rendering-won-46a349fadb52

---

### What is the extent of your experience with Promises and/or their polyfills?

Possess working knowledge of it. A promise is an object that may produce a single value some time in the future: either a resolved value, or a reason that it's not resolved (e.g., a network error occurred). A promise may be in one of 3 possible states: fulfilled, rejected, or pending. Promise users can attach callbacks to handle the fulfilled value or the reason for rejection.

Some common polyfills are `$.deferred`, Q and Bluebird but not all of them comply to the specification. ES2015 supports Promises out of the box and polyfills are typically not needed these days.

###### References

* https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-promise-27fc71e77261

---

### What are the pros and cons of using Promises instead of callbacks?

**Pros**

* Avoid callback hell which can be unreadable.
* Makes it easy to write sequential asynchronous code that is readable with `.then()`.
* Makes it easy to write parallel asynchronous code with `Promise.all()`.

**Cons**

* Slightly more complex code (debatable).
* In older browsers where ES2015 is not supported, you need to load a polyfill in order to use it.

---

### What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?

Some examples of languages that compile to JavaScript include CoffeeScript, Elm, ClojureScript, PureScript and TypeScript.

Advantages:

* Fixes some of the longstanding problems in JavaScript and discourages JavaScript anti-patterns.
* Enables you to write shorter code, by providing some syntactic sugar on top of JavaScript, which I think ES5 lacks, but ES2015 is awesome.
* Static types are awesome (in the case of TypeScript) for large projects that need to be maintained over time.

Disadvantages:

* Require a build/compile process as browsers only run JavaScript and your code will need to be compiled into JavaScript before being served to browsers.
* Debugging can be a pain if your source maps do not map nicely to your pre-compiled source.
* Most developers are not familiar with these languages and will need to learn it. There's a ramp up cost involved for your team if you use it for your projects.
* Smaller community (depends on the language), which means resources, tutorials, libraries and tooling would be harder to find.
* IDE/editor support might be lacking.
* These languages will always be behind the latest JavaScript standard.
* Developers should be cognizant of what their code is being compiled to — because that is what would actually be running, and that is what matters in the end.

Practically, ES2015 has vastly improved JavaScript and made it much nicer to write. I don't really see the need for CoffeeScript these days.

###### References

* https://softwareengineering.stackexchange.com/questions/72569/what-are-the-pros-and-cons-of-coffeescript

---

### What tools and techniques do you use for debugging JavaScript code?

* React and Redux
  * [React Devtools](https://github.com/facebook/react-devtools)
  * [Redux Devtools](https://github.com/gaearon/redux-devtools)
* JavaScript
  * [Chrome Devtools](https://hackernoon.com/twelve-fancy-chrome-devtools-tips-dc1e39d10d9d)
  * `debugger` statement
  * Good old `console.log` debugging

###### References

* https://hackernoon.com/twelve-fancy-chrome-devtools-tips-dc1e39d10d9d
* https://raygun.com/blog/javascript-debugging/

---

### What language constructions do you use for iterating over object properties and array items?

For objects:

* `for` loops - `for (var property in obj) { console.log(property); }`. However, this will also iterate through its inherited properties, and you will add an `obj.hasOwnProperty(property)` check before using it.
* `Object.keys()` - `Object.keys(obj).forEach(function (property) { ... })`. `Object.keys()` is a static method that will lists all enumerable properties of the object that you pass it.
* `Object.getOwnPropertyNames()` - `Object.getOwnPropertyNames(obj).forEach(function (property) { ... })`. `Object.getOwnPropertyNames()` is a static method that will lists all enumerable and non-enumerable properties of the object that you pass it.

For arrays:

* `for` loops - `for (var i = 0; i < arr.length; i++)`. The common pitfall here is that `var` is in the function scope and not the block scope and most of the time you would want block scoped iterator variable. ES2015 introduces `let` which has block scope and it is recommended to use that instead. So this becomes: `for (let i = 0; i < arr.length; i++)`.
* `forEach` - `arr.forEach(function (el, index) { ... })`. This construct can be more convenient at times because you do not have to use the `index` if all you need is the array elements. There are also the `every` and `some` methods which will allow you to terminate the iteration early.

Most of the time, I would prefer the `.forEach` method, but it really depends on what you are trying to do. `for` loops allow more flexibility, such as prematurely terminate the loop using `break` or incrementing the iterator more than once per loop.

---

### Explain the difference between mutable and immutable objects.

* What is an example of an immutable object in JavaScript?
* What are the pros and cons of immutability?
* How can you achieve immutability in your own code?

TODO

---

### Explain the difference between synchronous and asynchronous functions.

Synchronous functions are blocking while asynchronous functions are not. In synchronous functions, statements complete before the next statement is run. In this case the program is evaluated exactly in order of the statements and execution of the program is paused if one of the statements take a very long time.

Asynchronous functions usually accept a callback as a parameter and execution continues on the next line immediately after the asynchronous function is invoked. The callback is only invoked when the asynchronous operation is complete and the call stack is empty. Heavy duty operations such as loading data from a web server or querying a database should be done asynchronously so that the main thread can continue executing other operations instead of blocking until that long operation to complete (in the case of browsers, the UI will freeze).

---

### What is event loop? What is the difference between call stack and task queue?

The event loop is a single-threaded loop that monitors the call stack and checks if there is any work to be done in the task queue. If the call stack is empty and there are callback functions in the task queue, a function is dequeued and pushed onto the call stack to be executed.

If you haven't already checked out Philip Robert's [talk on the Event Loop](https://2014.jsconf.eu/speakers/philip-roberts-what-the-heck-is-the-event-loop-anyway.html), you should. It is one of the most viewed videos on JavaScript.

###### References

* https://2014.jsconf.eu/speakers/philip-roberts-what-the-heck-is-the-event-loop-anyway.html
* http://theproactiveprogrammer.com/javascript/the-javascript-event-loop-a-stack-and-a-queue/

---

### Explain the differences on the usage of `foo` between `function foo() {}` and `var foo = function() {}`

The former is a function declaration while the latter is a function expression. The key difference is that function declarations have its body hoisted but the bodies of function expressions are not (they have the same hoisting behaviour as variables). For more explanation on hoisting, refer to the question above on hoisting. If you try to invoke a function expression before it is defined, you will get an `Uncaught TypeError: XXX is not a function` error.

**Function Declaration**

```js
foo(); // 'FOOOOO'
function foo() {
  console.log('FOOOOO');
}
```

**Function Expression**

```js
foo(); // Uncaught TypeError: foo is not a function
var foo = function() {
  console.log('FOOOOO');
};
```

###### References

* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function

---

### What are the differences between variables created using `let`, `var` or `const`?

Variables declared using the `var` keyword are scoped to the function in which they are created, or if created outside of any function, to the global object. `let` and `const` are _block scoped_, meaning they are only accessible within the nearest set of curly braces (function, if-else block, or for-loop).

```js
function foo() {
  // All variables are accessible within functions.
  var bar = 'bar';
  let baz = 'baz';
  const qux = 'qux';

  console.log(bar); // bar
  console.log(baz); // baz
  console.log(qux); // qux
}

console.log(bar); // ReferenceError: bar is not defined
console.log(baz); // ReferenceError: baz is not defined
console.log(qux); // ReferenceError: qux is not defined

if (true) {
  var bar = 'bar';
  let baz = 'baz';
  const qux = 'qux';
}
// var declared variables are accessible anywhere in the function scope.
console.log(bar); // bar
// let and const defined variables are not accessible outside of the block they were defined in.
console.log(baz); // ReferenceError: baz is not defined
console.log(qux); // ReferenceError: qux is not defined
```

`var` allows variables to be hoisted, meaning they can be referenced in code before they are declared. `let` and `const` will not allow this, instead throwing an error.

```js
console.log(foo); // undefined

var foo = 'foo';

console.log(baz); // ReferenceError: can't access lexical declaration 'baz' before initialization

let baz = 'baz';

console.log(bar); // ReferenceError: can't access lexical declaration 'bar' before initialization

const bar = 'bar';
```

Redeclaring a variable with `var` will not throw an error, but 'let' and 'const' will.

```js
var foo = 'foo';
var foo = 'bar';
console.log(foo); // "bar"

let baz = 'baz';
let baz = 'qux'; // Uncaught SyntaxError: Identifier 'baz' has already been declared
```

`let` and `const` differ in that `let` allows reassigning the variable's value while `const` does not.

```js
// This is fine.
let foo = 'foo';
foo = 'bar';

// This causes an exception.
const baz = 'baz';
baz = 'qux';
```

###### References

* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let
* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var
* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const

---

### What are the differences between ES6 class and ES5 function constructors?

TODO

---

### Can you offer a use case for the new arrow => function syntax? How does this new syntax differ from other functions?

TODO

---

### What advantage is there for using the arrow syntax for a method in a constructor?

TODO

---

### What is the definition of a higher-order function?

A higher-order function is any function that takes one or more functions as arguments, which it uses to operate on some data, and/or returns a function as a result. Higher-order functions are meant to abstract some operation that is performed repeatedly. The classic example of this is `map`, which takes an array and a function as arguments. `map` then uses this function to transform each item in the array, returning a new array with the transformed data. Other popular examples in JavaScript are `forEach`, `filter`, and `reduce`. A higher-order function doesn't just need to be manipulating arrays as there are many use cases for returning a function from another function. `Array.prototype.bind` is one such example in JavaScript.

**Map**

Let say we have an array of names which we need to transform each string to uppercase.

```js
const names = ['irish', 'daisy', 'anna'];
```

The imperative way will be as such:

```js
const transformNamesToUppercase = function(names) {
  const results = [];
  for (let i = 0; i < names.length; i++) {
    results.push(names[i].toUpperCase());
  }
  return results;
};
transformNamesToUppercase(names); // ['IRISH', 'DAISY', 'ANNA']
```

Use `.map(transformerFn)` makes the code shorter and more declarative.

```js
const transformNamesToUppercase = function(names) {
  return names.map(name => name.toUpperCase());
};
transformNamesToUppercase(names); // ['IRISH', 'DAISY', 'ANNA']
```

###### References

* https://medium.com/javascript-scene/higher-order-functions-composing-software-5365cf2cbe99
* https://hackernoon.com/effective-functional-javascript-first-class-and-higher-order-functions-713fde8df50a
* https://eloquentjavascript.net/05_higher_order.html

---

### Can you give an example for destructuring an object or an array?

Destructuring is an expression available in ES6 which enables a succinct and convenient way to extract values of Objects or Arrays, and place them into distinct variables.

**Array destructuring**

```js
// Variable assignment.
const foo = ['one', 'two', 'three'];

const [one, two, three] = foo;
console.log(one); // "one"
console.log(two); // "two"
console.log(three); // "three"
```

```js
// Swapping variables
let a = 1;
let b = 3;

[a, b] = [b, a];
console.log(a); // 3
console.log(b); // 1
```

**Object destructuring**

```js
// Variable assignment.
const o = { p: 42, q: true };
const { p, q } = o;

console.log(p); // 42
console.log(q); // true
```

###### References

* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment
* https://ponyfoo.com/articles/es6-destructuring-in-depth

---

### ES6 Template Literals offer a lot of flexibility in generating strings, can you give an example?

TODO

---

### Can you give an example of a curry function and why this syntax offers an advantage?

Currying is a pattern where a function with more than one parameter is broken into multiple functions that, when called in series, will accumulate all of the required parameters one at a time. This technique can be useful for making code written in a functional style easier to read and compose. It's important to note that for a function to be curried, it needs to start out as one function, then broken out into a sequence of functions that each take one parameter.

```js
function curry(fn) {
  if (fn.length === 0) {
    return fn;
  }

  function _curried(depth, args) {
    return function(newArgument) {
      if (depth - 1 === 0) {
        return fn(...args, newArgument);
      }
      return _curried(depth - 1, [...args, newArgument]);
    };
  }

  return _curried(fn.length, []);
}

function add(a, b) {
  return a + b;
}

var curriedAdd = curry(add);
var addFive = curriedAdd(5);

var result = [0, 1, 2, 3, 4, 5].map(addFive); // [5, 6, 7, 8, 9, 10]
```

###### References

* https://hackernoon.com/currying-in-js-d9ddc64f162e

---

### What are the benefits of using spread syntax and how is it different from rest syntax?

ES6's spread syntax is very useful when coding in a functional paradigm as we can easily create copies of arrays or objects without resorting to `Object.create`, `slice`, or a library function. This language feature is used often in Redux and rx.js projects.

```js
function putDookieInAnyArray(arr) {
  return [...arr, 'dookie'];
}

const result = putDookieInAnyArray(['I', 'really', "don't", 'like']); // ["I", "really", "don't", "like", "dookie"]

const person = {
  name: 'Todd',
  age: 29,
};

const copyOfTodd = { ...person };
```

ES6's rest syntax offers a shorthand for including an arbitrary number of arguments to be passed to a function. It is like an inverse of the spread syntax, taking data and stuffing it into an array rather than unpacking an array of data, and it works in function arguments, as well as in array and object destructuring assignments.

```js
function addFiveToABunchOfNumbers(...numbers) {
  return numbers.map(x => x + 5);
}

const result = addFiveToABunchOfNumbers(4, 5, 6, 7, 8, 9, 10); // [9, 10, 11, 12, 13, 14, 15]

const [a, b, ...rest] = [1, 2, 3, 4]; // a: 1, b: 2, rest: [3, 4]

const { e, f, ...others } = {
  e: 1,
  f: 2,
  g: 3,
  h: 4,
}; // e: 1, b: 2, others: { g: 3, h: 4 }
```

###### References

* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax
* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/rest_parameters
* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment

---

### How can you share code between files?

TODO

---

### Why you might want to create static class members?

TODO

---

### Other Answers

* http://flowerszhong.github.io/2013/11/20/javascript-questions.html

## Related

If you are interested in how data structures are implemented, check out [Lago](https://github.com/yangshun/lago), a Data Structures and Algorithms library for JavaScript. It is pretty much still WIP but I intend to make it into a library that is able to be used in production and also a reference resource for revising Data Structures and Algorithms.

---

## Contributing

Feel free to make pull requests to correct any mistakes in the answers or suggest new questions.
