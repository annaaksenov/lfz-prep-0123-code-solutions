# prep-css-display

Using the `display` property to set elements to display on the page in three different formats.

## Before You Begin

Be sure to check out a new branch from `main` for this exercise. Detailed instructions can be found [**here**](../../guides/starting-an-exercise).

## Quiz

After completing this exercise, you should be able to discuss or answer the following questions:

- What are some characteristics of `block`?
- What are some characteristics of `inline`?
- What are some characteristics of `inline-block`?

## Exercise

1. Open the provided `index.html` file and have a look at the code.

#### Block

1. Read about the [`block` display type](https://www.w3schools.com/cssref/pr_class_display.asp) in the Property Values section. Be sure to keep this link open, because it contains the information on all the other display types covered in this exercise as well.

1. In your `index.html` create a `<div>` element with the following child text node:

    ```html
    <div>I am a div and by default I am block, which means I take up all the space I can horizontally.</div>
    ```

1. To be able to see the boundaries of the `<div>` element, create a CSS rule for the `<div>` element with the following CSS:

    ```css
    border: 4px solid blue;
    ```

    ![Example Block](assets/css-display-block.png)

    As you can see, the border of your `<div>` shows that it takes up all the space it can horizontally, along with creating a new line.  The default display type of a `<div>` element is `block`.

#### Inline

Another very common display type is `inline`.  It is very useful when adding children to an html element which do not need to create a new line, and only take up as much space as needed.

1. Read about the [`inline` display type](https://www.w3schools.com/cssref/pr_class_display.asp) in the Property Values section.

1. In your `index.html` create a `<div>` element with the following children and text nodes:

    ```html
    <div>
      I am a div but I have <span>span elements inside me</span>.
      Span elements are <span>display inline by default</span>,
      so they only take up as much as space as they need.
    </div>
    ```

1. To be able to see the boundaries of the `<span>` element, create a CSS rule for the `<span>` element with the following CSS:

    ```css
    border: 4px solid green;
    ```

    ![Example Span in Block](assets/css-display-span-in-block.png)

    As you can see, the border of your `<div>` shows that it takes up all the space it can horizontally, and yet the `<span>` elements size is dictated by the size of its content. The default display type of a `<span>` element is `inline`.

1. Another very important aspect of elements with the display `inline` property is that their height or width cannot be changed using css.  Add the following CSS to the CSS rule targeting `<span>` elements, and notice how it takes **no** effect:

    ```css
    height: 100px;
    width: 100px;
    ```

    ![Example Span In Block](assets/css-display-span-in-block.png)

#### Inline-Block

The display type `inline-block` is a hybrid of `block` and `inline`.

1. Read about the [`inline-block` display type](https://www.w3schools.com/cssref/pr_class_display.asp) in the Property Values section.

1. In your `index.html` create a `<div>` element with the following children:

    ```html
    <div>
      <button>Hello!</button>
      <button>Buttons are</button>
      <button>Inline Block</button>
      <button>By Default</button>
    </div>
    ```

1. To be able to see the boundaries of the `<button>` element, create a CSS rule for the `<button>` element with the following CSS:

    ```css
    border: 4px solid red;
    height: 40px;
    width: 200px;
    ```

    ![Example Inline Block](assets/css-display-inline-block.png)

    As you can see, the border of the `<div>` shows that it takes up all the space it can horizontally, and yet the `<button>` elements line up side by side *and* their height and width can be dictated by a css property. The default display type of a `<button>` element is `inline-block`.

#### Using Inline

In this section of the exercise, we will be demonstrating the display `inline` property with a common use case.


1. In your `index.html` create a `<ul>` element with the following children.

    ```html
    <ul>
      <li>
        Home
      </li>
      <li>
        Products
      </li>
      <li>
        About Us
      </li>
      <li>
        Contact Us
      </li>
    </ul>
    ```

    ![Example initial list example](assets/css-display-initial-list-example.png)

1. To be able to see the boundaries of the `<ul>` element, create a CSS rule for the `<ul>` element with the following CSS:

    ```css
    border: 4px solid purple;
    ```

1. To be able to see the boundaries of the `<li>` element, create a CSS rule for the `<li>` element with the following CSS:

    ```css
    border: 4px solid magenta;
    ```

    ![Example Output 5](assets/css-display-initial-list-highlight.png)

    As you can see, the border of your `<ul>` element and your `<li>` elements show that they take up all the space they can horizontally, along with creating a new line.  The default display property of a these elements is display `block`.

1. Add the following CSS to the CSS rule for `<li>` elements:

    ```css
    display: inline;
    ```

    ![Example Single Line List](assets/css-display-single-line-list.png)

    As you can see the `<li>` elements now line up side by side, and only take up as much space as needed.

## Submitting Your Solution

When your solution is complete, submit a Pull Request on GitHub. Detailed instructions can be found [**here**](../../guides/submitting-your-solution).
