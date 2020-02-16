# css-lecture

Here's a recording of the lecture that I ran for Flatiron School students on 10/04/2019: [video](https://www.youtube.com/watch?v=p_dDWuKu70c&feature=youtu.be).

## For starters: world without CSS
Try this (it removes all css in a website):

```js
  document.querySelectorAll('[style]')
    .forEach(el => el.removeAttribute('style'));
  document.querySelectorAll('link[rel="stylesheet"]')
    .forEach(el => el.parentNode.removeChild(el));
  document.querySelectorAll('style')
    .forEach(el => el.parentNode.removeChild(el));
```
Press `option + command + j` then paste this code in and press `enter`

## WARM UP: QUIZ
#### Open ./quiz/index.html in your browser.
Or play here: <http://cssisfun.surge.sh/>

Also: Bootstrap, Semantic UI, Materialize, Deque -> what is it? why would I (not) use it?

## The Box Model
4 elements of the box model:
- margin - the area outside the border (it is transparent);
- border - it goes around the padding and content;
- padding - the area around the content (it is transparent);
- content - the content of the box, where text and images appear;

## The Cascade vs Specificity vs Inheritance vs !important
* **Cascade**: CSS is a cascade (a type of algorithm). At a very low level, it means that that the order of CSS rules matter; meaning, if you define a background color of a div in two places, the color that comes last will be applied;
* **Specificity**: however, more important than the cascading character of css is the rule of specificity; CSS will take more seriously the requsts that are more specific; here's the hierarchy of specificity (from the most to the least): 
element selector -> class selector -> id selector
**note**: inline CSS is more specific than external file, which is why it's easy to overwrite external libraries;
PS: Specificity is set up with point system -- each declaration is evaluated in points, then compared and the winners take it all! For instance, if you declare styling inline, this declaration gets 1000 points from the get-go (for real), as opposed to 0 when declared in an outside stylesheet;
* **Inheretance**: now, some elements inherit styling from their parents while others don't; for instance, color and font will be inherited by children but width and height will not! You can play with inheritance by using an ``inherit`` attribute!
* **!important**: now, you can override all rules using the value of ``!important``; however, beware: you will enter the long-term css debugging hell if you invite this value without an absolute desperate necessity;  

## Cheat sheets:
1. Button generator: <https://www.bestcssbuttongenerator.com/#/3>
2. 10 animations generators (including fancy spinners you will love while doing React): <https://www.hongkiat.com/blog/css3-animation-tools/>
3. More animations: <https://sarthology.github.io/Animatopy/>
4. CSS generator: <http://angrytools.com/css-generator/>
5. Another CSS generator: <https://webcode.tools/css-generator/>
6. Gradient generator: <http://angrytools.com/gradient/>
7. Grid templates: <https://gridbyexample.com/examples/>
8. 

## Practice:
1. CSS: <https://flukeout.github.io/>
2. Flexbox: <https://flexboxfroggy.com/>
3. Grid: <http://cssgridgarden.com/>

## Read more:
1. All attributes: <https://tympanus.net/codrops/css_reference/>
2. All selectors and how to chain them: <https://www.w3schools.com/cssref/css_selectors.asp>
3. All about grid: <https://css-tricks.com/snippets/css/complete-guide-grid/>
4. All about flexbox: <https://css-tricks.com/snippets/css/a-guide-to-flexbox/>
5. 20 tricks to make your life easier: <https://www.webdesignerdepot.com/2016/10/20-essential-css-tricks-every-designer-should-know/>
6. Grid vs Flexbox: <https://medium.com/youstart-labs/beginners-guide-to-choose-between-css-grid-and-flexbox-783005dd2412>

## Accessibility tools:
1. Font sizes: [em](https://www.w3.org/TR/WCAG20-TECHS/C14.html), [% sizes](https://www.w3.org/TR/WCAG20-TECHS/C12.html), [named sizes](https://www.w3.org/TR/WCAG20-TECHS/C13.html)
    * play with them here: <https://www.w3schools.com/cssref/playit.asp?filename=playcss_font-size&preval=smaller>
2. Color contrast explanation: <https://a11yproject.com/posts/what-is-color-contrast/>
    * Color contrast checker: <https://colorable.jxnblk.com/d7cdca/252f32>
    * Color contrast generator: <https://learnui.design/tools/accessible-color-generator.html>
3. :focus property <https://a11yproject.com/posts/never-remove-css-outlines/>
4. Deque Pattern Library (instead of bootstrap or materialize): <https://pattern-library.dequelabs.com/>
5. ***ADVANCED*** :maximum-scale property <https://a11yproject.com/posts/never-use-maximum-scale/>

## DESSERT: ENJOY!
1. This painting was made entirely with CSS: <http://diana-adrianne.com/purecss-francine/>
2. All made with CSS: <https://a.singlediv.com/>
3. Zen Garden: <http://cssgridgarden.com/>
4. Mind-blowing CSS projects: <https://www.webdesignerdepot.com/2017/09/11-experimental-css-projects-thatll-blow-your-mind/>
