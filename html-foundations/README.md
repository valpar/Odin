# HTML foundations

## Html tags and elements

`<p>some text content</p>`

`<p>` is the opening tag.
some text content represents content wrapped within the opening and closing tags.
`</p>` is the closing tag.

### Void elements

Some HTML elements do not have a closing tag. These elements just have a single tag, like: `<br/>` or `<img/>`.

## 2. Html boilerplate

1. How to write the basic boilerplate for an HTML document.
2. How to open HTML documents in your browser.

It is worth noting that we named our HTML file index. We should always name the HTML file that will contain the homepage of our website index.html. This is because web servers will by default look for an index.html page when users land on our websites – and not having one will cause big problems.

### DOCTYPE

Every HTML page starts with a doctype declaration. The doctype’s purpose is to tell the browser what version of HTML it should use to render the document. The latest version of HTML is HTML5, and the doctype for that version is `<!DOCTYPE html>`.

### HTML element

After we declare the doctype, we need to provide an `<html>` element. This is what’s known as the root element of the document, meaning that every other element in the document will be a descendant of it.

#### Lang attribute

`lang` specifies the language of the text content in that element. This attribute is primarily used for improving accessibility of the webpage. It allows assistive technologies, for example screen readers, to adapt according to the language and invoke correct pronunciation.

### Head element

The `<head>` element is where we put important meta-information about our webpages, and stuff required for our webpages to render correctly in the browser. Inside the `<head>` , we should not use any element that displays content on the webpage.

#### Meta element

We should always have the `<meta>` tag with the charset encoding of the webpage in the `<head>` element: `<meta charset="UTF-8">`.

Setting the encoding is very important because it ensures that the webpage will display special symbols and characters from different languages correctly in the browser.

#### Title element

Another element we should always include in the head of an HTML document is the `<title>` element:

`<title>My First Webpage</title>`

The `<title>` element is used to give webpages a human-readable title, which is displayed in our webpage’s browser tab. For example, if you look at the current tab’s name of your browser, it will read “HTML Boilerplate | The Odin Project”; this is the `<title>` of the current .html file.

If we didn’t include a `<title>` element, the webpage’s title would default to its file name. In our case that would be index.html, which isn’t very meaningful for users; this would make it very difficult to find our webpage if the user has many browser tabs open.

#### Body element

The final element needed to complete the HTML boilerplate is the `<body>` element. This is where all the content that will be displayed to users will go - the text, images, lists, links, and so on.

### VScode shortcut

VSCode has a built-in shortcut you can use for generating all the boilerplate in one go. Please note that this shortcut only works while editing a file with the .html extension or a text file with the HTML language already selected. To trigger the shortcut, delete everything in the index.html file and just enter ! on the first line. This will bring up a couple of options. Press the Enter key to choose the first one, and voila, you should have all the boilerplate populated for you.
