# HTML Images
We use the ```<img>``` element to place images into a web page.  The ```src``` attribute must have a path to the image on your web server.  The src element is the only required element, but it is a best practice to also include an alternate description of the image for people with vision disabilities can use
also use the web page.

```html
<img src="img/earth.jpg" alt="Photo of earth from space"/>
```

![Photo of earch from space](img/earth.jpg)

## Changing the Image Size
You can also add a ```width``` and a ```height``` to control the horizontal (x) and the vertical (y) dimensions of an image.

In this example, we will shrink the image down to 50X50 pixels:
```html
<img src="img/earth.jpg" alt="Photo of earth from space" width="100" height="100"/>
```

<img src="https://www.coderdojotc.org/web-ux/intro-to-html/img/earth.jpg" alt="Photo of earth from space" width="100" height="100"/>

## Relative vs Absolute Paths
There are two ways to reference an image.  Both methods have pros and cons.  If you are deploying a single web site that you want consistent behavior, it is best to include all the images in your own web site and then use a relative path to the images.  If you want to share images between multiple areas of the web site they should be place in a common folder, typically named the ```img``` folder.  Relative paths start with that folder name.

The alternative is to directly reference images on the web using a full URL that starts with ```http://```.  This has the advantage of being portable as long as that the path to the image does not change.  However, you sometimes can't guarantee that a remote web site will not move images around or change their file names.  So to be fully in control of your image references, use a relative path.

## Best Practice for Fast Web Page Loading
You also want to be aware of the size of your images.  For most web pages, a size of around 10K for small images is fine.  Most cameras today store images in large files of several megabytes.  Make sure you use a tool to reduce the size of these images before you add them to your web page.


