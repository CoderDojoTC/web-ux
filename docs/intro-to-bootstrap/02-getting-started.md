# Getting Started

(with Bootstrap 4)

It's easy to add Bootstrap to our webpage. Just like how we can reference CSS, and JavaScript files from our HTML file, we can do the same to add Bootstrap, except the CSS and JavaScript is a file from the internet. 

You can get started on your favorite online/offline code editor.

## CSS

In your HTML file, add the following `<link>` element in the contents of your `<head>` element.

```html
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
```

## Javascript


Bootstrap requires some JavaScript packages to work. Add these `<script>`s at the end of your page, before the end of your `<body>`. This will tell the web browser to load the HTML content before the JavaScript, and allow the web page to load faster.

```html
<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM" crossorigin="anonymous"></script>
```

## Starter Template

This starter template allows you to quickly create a Bootstrap page.

```html
<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">

    <title>Hello, world!</title>
  </head>
  <body>
    <h1>Hello, world!</h1>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM" crossorigin="anonymous"></script>
  </body>
</html>
```

## Meta Tag

You may have noticed something unfamiliar, the `<meta>` tag with its attribute, `name` value of `"viewport"`.
This is used to ensure our CSS scales the same across all devices.

```html
<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
```

## HTML example

Add the following to our HTML document, and examine what happens when we change the size of our browser.


```html
<div class="jumbotron text-center">
  <h1>My First Bootstrap Page</h1>
  <p>Resize this responsive page to see the effect!</p>
</div>

<div class="container">
  <div class="row">
    <div class="col-sm-4">
      <h3>Column 1</h3>
      <p>Lorem ipsum dolor..</p>
    </div>
    <div class="col-sm-4">
      <h3>Column 2</h3>
      <p>Lorem ipsum dolor..</p>
    </div>
    <div class="col-sm-4">
      <h3>Column 3</h3>
      <p>Lorem ipsum dolor..</p>
    </div>
  </div>
</div>
```

## Note on Content Delivery Networks (CDN)

What's a CDN and what's up with this "*integrity check*"?


You may recall how we imported the Bootstrap CSS file.

```html
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
```

### Breaking it down

#### Web Resources

We can see that the link has an attribute, `href` with the value, `"https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css"`. 

This `href` "points" to a web resource (a file) named `bootstrap.min.css`

#### Web page loading

A *Content Delivery Network* (CDN) is a central point where a client (such as a web browser) can request a web file. The CDN can automatically pick the geographically closest, available web server that has the file, in order to improve web page load times. Companies and web developers use CDNs all the time to host *static content*, files that are not expected to change.

For example, say I am on the East Coast, Boston, Massachusetts, and using my laptop (the *client*), I access my friend's photo sharing website, which he hosts entirely on a computer (the *host*) in his home on the West Coast, San Francisco, California. The speed at which my friend can transfer these photos to my computer is not only limited by the network speed of my friend's home-internet, but also the distance between the client and the host. Specifically, the speed of data transfer between a client, and host is limited by the *speed of light* (3 * 10^8 m/s in a vacuum). 

For example, the distance between New York and Paris (in a straight line) is about 5,800 kilometers. In order for light to travel that distance and back, it would take *40 milliseconds*. We consider this to be a theoretical minimum ping between two locations. Real-world pings are slower due to many reasons such as the real-distance of the fiber optic cables, the speed of light in the cable material, delays in routing services, etc.

## Resources

- [Bootstrap Offical Documentation Getting Started](https://getbootstrap.com/docs/4.3/getting-started/introduction/)
- [W3 Schools Bootstrap 4 Tutorial](https://www.w3schools.com/bootstrap4/)
