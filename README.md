# Basics of HTML and CSS

# HTML

For an introduction to HTML please go to [WebPlatform](http://docs.webplatform.org/wiki/html/tutorials).

Recommendations:

1. **The Basics of HTML:** create a basic `.html` file and experiment a little bit with it (add titles, images, tables, lists, ...).
2. **Doctypes and Validations:** Learn how to write valid, and semantic markup [HTML VAlidation](https://docs.webplatform.org/wiki/guides/html_validation) ADD EXERCISE
3. **The HTML head:** ADD A RESOURCE EXPLAINING HEAD; METATAGS; LINKS; SCRIPTS.
4. **The HTML body:** ADD A LINK TO NEW HTML5 TAG SEMANTICS
5. **ACCESSIBILITY** ADD LINK TO ACCESSIBILITY

By now, you should have an `html` file with several examples of how to create lists, tables, add images, headers, etc. All the markup is syntactically valid, is semantic, passes the HTML validator, and is accessible.

# CSS

* Create a basic [index.html](https://raw.githubusercontent.com/h5bp/html5-boilerplate/master/index.html) file (example provided).
* Create an empty style.css file and link it to the index.html using [<link> tag](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/link#Examples).
* Include [normalize.css](http://necolas.github.io/normalize.css/) before your style.css to fix cross-browser problems.
* Add a basic page structure using HTML as it’s described in the following picture:

![alt text](images/html5-structure.png "HTML5 structure")

## Rules
  
### Selectors and properties 
![alt text](images/anatomy-of-a-css-rule.gif "Anatomy of a CSS rule")

* [Brief of CSS selectors](http://www.sitepoint.com/web-foundations/css-selectors/)
* [CSS3 selectors sheet](http://www.w3.org/TR/css3-selectors/)
* [Play a little game to consolidate your knowledge](http://flukeout.github.io/)
* [Bookmark the following list of properties for future reference](http://ref.openweb.io/CSS/)
* [Bookmark a reference of CSS Vocabulary](http://pumpula.net/p/apps/css-vocabulary/)
* Now write some code and:
    * Add background to the header, footer, aside and nav.
    * Add a global font definition (at html element) with a value of 14px, using a font-family you like.
    * Make the header and footer text centered.
    
### Specificity        
[Learn about CSS Specificity (basically how the rules override others)](http://www.w3.org/TR/CSS21/cascade.html#specificity)

* [Experiment specificity right now using CSS3 selectors](http://specificity.keegan.st/)
* Now add classes to the different HTML tags with the following names:
    * To &lt;header&gt;  add class .header
    * To &lt;footer&gt;  add class .footer
    * To &lt;section&gt;  add class .content
    * To &lt;nav&gt;  add class  .navigation
    * To &lt;aside&gt;  add class  .sidebar
* Using the new added classes figure out how to override:
    * .header must define a font-size: 46px;
    * .footer must define a font-size: 10px;
    * .content must define a font-size: 14px;
    * .navigation must define a font-size: 12px;
    * .sidebar must define a font-size: 10px;
* If the class attribute finish with **r (example header, footer)**, the background must be magenta.
* If the class attribute contain an **a (example nav)** but do NOT finish with r, the background must be blue.
* How could you add weight to the global font definition to override all the overrides provided by point c?
* Imagine you have something like class=”oh-no-inline-styles” style=”background:red” and you should change the background to green but without changing the inline style, How could you accomplish this?

### The Box Model
* [Learn about the Box Model (how the browser calculate boxes size)](http://www.w3.org/TR/CSS21/box.html)
  * [Play with it here changing width / margin / padding / box-sizing](http://dabblet.com/gist/2986528)
* [How to alter the box model calculations](http://quirksmode.org/css/user-interface/boxsizing.html)
* [Extra about box-sizing](http://adamschwartz.co/magic-of-css/chapters/1-the-box/)
  * Use the playground provided above to change *box-sizing* and see the changes.

### Layout

#### The display property
* [Learn how to handle the display property (block, inline, inline-block, none)](http://learnlayout.com/display.html)
* [An extra documentation (only read display property for now)](http://adamschwartz.co/magic-of-css/chapters/2-layout/)
  * Now modify your CSS to reach something similar to the initial layout asked. You will need to be smart with the use of *display: inline-block*.
  
#### Layout systems  
* [Learn how to create your own layout system](http://www.adamkaplan.me/grid/)
  * [Checkout floats and fully understand them](http://alistapart.com/article/css-floats-101)
  * [Review your knowledge about CSS relative units](http://alistapart.com/article/love-the-boring-bits-of-css)
* Using your own layout system, implement the following page (only desktop).
  ![alt text](images/example-layout.png)
  * When the user **:hover** the right side black box (observe at middle right of the screen shot) it must show a “hello world” message and go back when move the mouse out. To accomplish this [Learn about CSS position](http://learnlayout.com/position.html).

### Media queries
* [Learn Media Queries](http://css-tricks.com/css-media-queries/) and Adapt the given layout to be ready for mobile screens using the following design as guide [example](http://mediaqueri.es/ity/).

