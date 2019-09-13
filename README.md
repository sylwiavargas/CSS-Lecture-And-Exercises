# css-lecture

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
#### Open ./quiz.html in your browser.

Also: Bootstrap, Semantic UI, Materialize, Deque -> what is it? why would I (not) use it?

## The Box Model
4 elements of the box model:
- margin - the area outside the border (it is transparent);
- border - it goes around the padding and content;
- padding - the area around the content (it is transparent);
- content - the content of the box, where text and images appear;

## Cheat sheets:
1. Button generator: <https://www.bestcssbuttongenerator.com/#/3>
2. 10 animations generators (including fancy spinners you will love while doing React): <https://www.hongkiat.com/blog/css3-animation-tools/>
3. CSS generator: <http://angrytools.com/css-generator/>
4. Another CSS generator: <https://webcode.tools/css-generator/>
5. Gradient generator: <http://angrytools.com/gradient/>
6. Grid templates: <https://gridbyexample.com/examples/>

## Practice:
1. CSS: <https://flukeout.github.io/>
2. Flexbox: <https://flexboxfroggy.com/>
3. Grid: <http://cssgridgarden.com/>

## Read more:
1. All attributes: <https://tympanus.net/codrops/css_reference/>
2. All about grid: <https://css-tricks.com/snippets/css/complete-guide-grid/>
3. All about flexbox: <https://css-tricks.com/snippets/css/a-guide-to-flexbox/>
4. 20 tricks to make your life easier: <https://www.webdesignerdepot.com/2016/10/20-essential-css-tricks-every-designer-should-know/>

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
