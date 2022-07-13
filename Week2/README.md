# Reading Material Start Week 2

## Agenda

These are the topics for week 2:

1. Responsiveness
   - Flexible organizing with flexbox
   - Using the grid layout
   - Responsive design with media queries
2. Advanced CSS
   - Pseudo class selectors
   - Pseudo elements

## 1. Responsiveness

By now you've had some practice with CSS. In the following sections you'll learn about some more essentials concepts in order to make sure that your webpages are responsive! In the modern age webpages are being accessed by many different devices with many different screen sizes which means that you as the developer need to write your CSS to support all those devices.

### Flexible organizing with flexbox

CSS is used to order and style HTML elements. A big part of this is organising elements in a visually attractive way. This can be done using `flexbox`.

What it does is helping you to think according to `grid-based web design`: elements are not randomly placed on the page, but are neatly organised along a grid.

Read the following to learn more about 'grid-based web design':

- [Introduction to grids in web design](https://webdesign.tutsplus.com/articles/a-comprehensive-introduction-to-grids-in-web-design--cms-26521)
- [Intro to Web Design Grids](https://www.youtube.com/watch?v=gjYZoPEk0ow)

Once you understand this way of thinking you'll know why it makes sense to use `flexbox`.

In order to make use of it we have to access it through the `display` CSS property:

```css
display: flex;
```

This will give us the `flexbox`-specific properties, so we can develop clean and organised CSS. Check the following links to understand how this is done:

- [CSS Flexbox in 100 Seconds](https://www.youtube.com/watch?v=K74l26pE4YA)
- [What is Flexbox and Why to Learn it](https://www.youtube.com/watch?v=CXSwNIPsyTs)
- [CSS Flexbox Course](https://www.youtube.com/watch?v=-Wlt8NRtOpo)

### Using the grid layout

The most recent addition to the css toolkit for organising your layout is using `display: grid`. Where every other layout always goes from top to bottom, grid allows you to create a two-dimensional layout.

The complete guide to grid by css-tricks is the go to guide, read it here:

- [CSS-tricks complete guide to grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

### Responsive design with media queries

Nowadays people use different devices to access websites: desktops, tablets and mobile phones of all different sizes. Responsive design is a way to put together a website so that it automatically scales its content and elements to match the screen size of the viewer. It prevents that images are larger than the screen width, so visitors on mobile devices will see a visually attractive website as well

For more information about responsive design, check this article: [Responsive Design](https://www.internetingishard.com/html-and-css/responsive-design/).

The primary way of making a responsive website is by writing custom CSS code that makes it so. This can be done using `media queries`: CSS instructions that only apply to certain screen sizes.

Learn more about media queries here:

- [Introduction to Media Queries](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Media_queries).
- [Learn CSS Media Query in 7 Minutes](https://www.youtube.com/watch?v=yU7jJ3NbPdA)

### Layouts

Now that you know about all the tools at your disposal it is time to look at how to create layouts, which are the most basic design of your app/website. It is important to always do this step first as any changes in the layout will affect all of the other parts in the website, whereas the smaller parts do not affect the overall layout.

Learn more about them here:

- [The fundamentals of css layouts](https://www.youtube.com/watch?v=yMEjLBKyvEg)

## 2. Advanced CSS

Now that we have covered everything that you will probably use with every webpage it is time to go over some advanced CSS that you will need to use in some more specific use cases.

### Pseudo class selectors

Every HTML element can be in different states. The default state is when an element is untouched, you already know how to style for this as that is the default styling.

```css
button {
  background-color: white;
}
```

There are times when a user interacts with an element. For example: clicking a button that opens another page. As frontend developers we need to give the user feedback on that particular action. When they place the mouse on top of the button it lights up (we call this a `hover state`). We need to write instructions for that to happen:

```css
button:hover {
  background-color: blue;
}
```

Like the hover state there are others as well: `click`, `focus`, `visited`, and more. For most of these element states we have special selectors that allow you to change the styling. Read the following article to learn about them. Once you have done that, try them out for yourself!

- [Pseudo class selectors](https://css-tricks.com/pseudo-class-selectors/)

### Pseudo elements

Next to pseudo class selectors there is also something called pseudo elements. This is a way that css can insert 'HTML elements' before or after what you are selecting which allows you to do some very powerful things without having to write any JavaScript (which we will learn about next week)! To do this you can write the following code:

```css
.required::after {
  content: "*";
}
```

This is an `::after` element which means that the html element will be placed directly after the HTML element. Conversely, you can use the `::before` element to place it directly before the element you targeted with your css. In this case any HTML element that has the css class `required` assigned to it will get an extra HTML element after it with the star. Have a look at the following video that goes into this and explains the use case that this css code solves:

- [CSS Pseudo Elements in 8 minutes](https://www.youtube.com/watch?v=OtBpgtqrjyo)

It may be a little unclear now what the real difference is between these two. The following video goes over that to get it clear in your mind:

- [Pseudo-Classes vs Pseudo-Elements in CSS](https://www.youtube.com/watch?v=0VDx1570X3U)

## Finished?

Are you finished with going through the materials? Nice job!!! If you feel ready to get practical, click [here](./MAKEME.md).
