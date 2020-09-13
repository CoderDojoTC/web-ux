# HTML Images
We use the ```<img>``` element to place images into a web page.  The ```src``` attribute must have a path to the image on your web server.  The src element is the only required element, but it is a best practice to also include an alternate description of the image for people with vision disabilities can use
also use the web page.

```html
<img src="img/earth.jpg" alt="Photo of earth from space"/>
```

![Photo of earch from space](img/earth.jpg)

## Changing the Image Size
You can also add a ```width``` and a ```height``` to control the horizontal (x) and the vertical (y) dimensions of an image.

```html
<img src="intro-to-html/img/earth.jpg" alt="Photo of earth from space" width="100" height="100"/>
```

![Photo of earch from space](img/earth.jpg) {: style="height:50px;width:50px"}

## Best Practice for Fast Web Page Loading
You also want to be aware of the size of your images.  For most web pages, a size of around 10K for small images is fine.  Most cameras today store images in large files of several megabytes.  Make sure you use a tool to reduce the size of these images before you add them to your web page.


