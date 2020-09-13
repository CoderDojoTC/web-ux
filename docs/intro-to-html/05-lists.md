# HTML Lists

HTML has several types of lists:

1. Unorder lists
2. Ordered Lists
3. Definition Lists

## Unordered Lists
This is just a simple list with markers called "bullets" at the front of every new list item.  We used the ```<ul>``` tag to start an unordered list and we use the ```<li>``` tag to specify each list item.

```html
<ul>
   <li>Apples</li>
   <li>Bananas</li>
   <li>Pears</li>
</ul>
```

<ul>
   <li>Apples</li>
   <li>Bananas</li>
   <li>Pears</li>
</ul>

## Ordered lists

<ol>
   <li>Apples</li>
   <li>Bananas</li>
   <li>Pears</li>
</ol>
```

<ol>
   <li>Apples</li>
   <li>Bananas</li>
   <li>Pears</li>
</ol>

## Definition lists
These are lists that have a definition title (```<dt>```) at the front of each item.  The item then has a definition description ```<dd>``` right after the title.  Each item can have it's own distinct label.  Definition lists are ideal for creating a dictionary list where the label

<dl>
  <dt>Engage</dt>
  <dd>Where we introdce our topic and any backround motivation.</dd>
  <dt>Elicit</dt>
  <dd>Where we ask the students what their prior knowledge and how it might be related to the new topic.</dd>
  <dt>Explore<dt>
  <dd>Where students get a chance to interact with the elements and try out some sample code.</dd>
  <dt>Explain<dt>
  <dd>Where we explain what each component does.</dd>
  <dt>Elaborate<dt>
  <dd>Where we dive into the details of how the components interact.</dd>
  <dt>Extend<dt>
  <dd>Where we ask students to extend the example code.</dd>
  <dt>Evaluate</dt>
  <dd>Where we check if the students compenhend the lesson</dd>
</dl>
