# HTML File Structure
HTML files all have a consistent structure of elements and attributes. In this lab we will take a look at this structure and see how the elements work together to describe the way a web page is laid out and rendered.

## Getting Started Template
Here is a standard template we will be using for our example programs.

```html
<!DOCTYPE html>
<html lang="en">
   <head>
      <meta charset="utf-8"/>
      <title>A simple HTML document</title>
    </head>
   <body>
      <p>Hello World!<p>
   </body>
</html>
```

## DOCTYPE
There are many varieties and versions of HTML files.  This line indicates that
this file conforms to the most common modern format: HTML 5.

## html
This is the root element.  The begin tag should be the second line of the file and the end tag the last line of the file.  The html element contains two parts.  The first is the head that hold the title and data about the content and the body has the page content itself.  The ```lang="en"``` tells web crawlers that the language of this web page is English.


## head
The head element contains information about the page content.  This includes the page title that appears on the browser tab.  It is a good best practice to pick a short but descriptive page title.  The ```<meta charset="utf-8"/>``` element indicates that the encoding character set is UTF-8.  This is the preferred format for encoding web pages.

## body
The body element contains the page content itself.  The elements within the body elements hold the structure of the web page and the text that is rendered within each element.

## Block and Inline Elements
The body element contains two types of elements:

1. **Block elements** always starts on a new line and takes up the full width available.  Block elements stretch out to the left and right as far as the layout permits.  Block elements are used to arrange large regions of page layout.
2. **Inline elements** do not start on a new line and it only take up as much width as necessary.  They are frequently used to change the way individual words are displayed within text blocks.  For example you can use an inline element to change the font or color of a few words within a line of text.

One of the tricky things about learning HTML layout is to understand the rules of how block and inline elements work together.

