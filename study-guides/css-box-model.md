In a document, or a website, each element is represented by a regular box. Each of the rectangular boxes has four edges: the margin edge, border edge, padding edge, and content edge. Let's take a look at the CSS Box Model.

## Box Model Components

![Image of CSS box model](https://upload.wikimedia.org/wikipedia/commons/7/7a/Boxmodell-detail.png)

Source: [Wikipedia](https://en.wikipedia.org/wiki/CSS_box_model)

- `width`: This refers to the width of the content area of the element.
- `height`: This refers to the height of the content area of the element.
- `padding`: Directly surrounding the content area of the element is the padding. The **padding** can be divided into four different properties: `padding-top`, `padding-right`, `padding-bottom`, and `padding-left`. Most web browsers give elements a default padding size of `0px`.
- `border`: The **border** is the space between the padding and margin. Developers can modify the `border-color`, `border-style`, and `border-width` of an element. These properties can also be specified to its 4 different edges: `border-top`, `border-right`, `border-bottom`, and `border-left`. Most web browsers give elements a default border size of `0px`.
- `margin`: The **margin** is the outermost space directly surrounding the border. The margin can be divided into four different properties: `margin-top`, `margin-right`, `margin-bottom`, and `margin-left`. Most web browsers give elements a default margin size of `16px`.

Some web browsers add default padding, border, and margin sizes. To ensure that elements appear in the exact same positioning on all browsers, developers often use the universal selector, `*`, to reset these property values to `0`.

There are a variety of ways to customize the margin, border, and padding size based on the top, bottom, left, and right edges. Let's take a look at a few examples in code:

```css
div {
  /* This: */
  margin: 20px;
  /* Is the same as: */
  margin-top: 20px;
  margin-right: 20px;
  margin-bottom: 20px;
  margin-left: 20px;

  /* This: */
  padding: 10px 20px;a
  /* Is the same as: */
  padding-top: 10px;
  padding-right: 20px;
  padding-bottom: 10px;
  padding-left: 20px;
}

h1 {
  /* This: */
  margin: 20px 10px 5px;
  /* Is the same as: */
  margin-top: 20px;
  margin-right: 10px;
  margin-bottom: 5px;
  margin-left: 10px;
}

h2 {
  /* This: */
  margin: 10px 20px;
  /* Is the same as: */
  margin-top: 10px;
  margin-right: 20px;
  margin-bottom: 10px;
  margin-left: 20px;
}
```

There are a variety of ways to customize the margin, border, and padding size based on the top, bottom, left, and right edges. Let's take a look at a few examples in code:

```css
div {
    /* This: */
    margin: 20px;
    /* Is the same as: */
    margin-top:20px;
    margin-right:20px;
    margin-bottom:20px;
    margin-left:20px;

    /* This: */
    padding: 10px 20px;
    /* Is the same as: */
    padding-top:10px;
    padding-right:20px;
    padding-bottom:10px;
    padding-left:20px;
}

h1 {
    /* This: */
    margin: 20px 10px 5px;
    /* Is the same as: */
    margin-top:20px;
    margin-right:10px;
    margin-bottom:5px;
    margin-left:10px;
}   

h2 {
    /* This: */
    margin: 10px 20px;
    /* Is the same as: */
    margin-top: 10px;
    margin-right: 20px;
    margin-bottom: 10px;
    margin-left: 20px;
}
```


:bangbang: **Tip**: For sizing, you can use a variety of units. The popular units are `em`, `%`, or `px`. Check out MDN Docs on [CSS values and units](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units).

You can learn more about the [CSS Box Model on MDN Doc](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model/Introduction_to_the_CSS_box_model).

## 🐞 Debugging with Chrome Developer Tools

Using a [Chrome](https://www.google.com/chrome/) browser? The DevTools on Chrome is a great resource to help you debug your code, visualize changes in HTML or CSS, and analyze the positioning of elements based on the box model.

![Gif on Chrome DevTools and element inspection](http://www.compjour.org/files/images/tutorials/devtools/inspecting-elements-perusing-the-dom.gif)

Source: [Computational Journalism](http://www.compjour.org/tutorials/elements-of-a-webpage/)

The DevTools in Chrome is very powerful. We highly recommend you take the time to check out Computational Journalism's tutorials on [elements of a webpage](http://www.compjour.org/tutorials/elements-of-a-webpage/) and [Chrome DevTools documentation](https://developer.chrome.com/docs/devtools/).
