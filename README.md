# developer-test

Please create a fork of this repository and modify corresponding testX.html file to resolve the items below. Then share us the link to the repository with solved items.

1. Tables

You've been sent a snippet from a spreadsheet, and have been asked to re-create it for display on the company's internal website.

Re-create the following spreadsheet using HTML, in a table appropriately captioned "Purchase Orders".

![Download it from: https://www.testdome.com/files/resources/19201/tabb.PNG](https://www.testdome.com/files/resources/19201/tabb.PNG)


```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Spreadsheet</title>
    <style>
      td {
        text-align: right;
        width: 33%;
      }
      td, th, table {
        border: 1px solid;
        border-collapse: collapse;
      }
      th {
        text-align: left;
      }
    </style>
  </head>
  <body>
    <table>  
      <thead>
      </thead>
      <tbody>
      </tbody>
    </table>
  </body>
</html>
```

2. Styling Links

Write CSS so that link ```<a href="http://www.testdome.com">Check documentation</a>``` and cursor looks like a question mark:

![Download it from https://www.testdome.com/files/resources/12362/1ea3e6cc-c0ce-4789-b806-ef753147d469.png](https://www.testdome.com/files/resources/12362/1ea3e6cc-c0ce-4789-b806-ef753147d469.png)


3. Image Gallery

An image gallery is a set of images with corresponding remove buttons. This is the HTML code for a gallery with two images:

```
<div class="image"> 
	<img src="https://goo.gl/kjzfbE" alt="First"> 
	<button class="remove">X</button> 
</div> 
<div class="image"> 
	<img src="https://goo.gl/d2JncW" alt="Second"> 
	<button class="remove">X</button> 
</div>
```
Implement the setup function that registers a click event handler and implements the following logic: When the button of class remove is clicked, its parent ```<div>``` element should be removed from the gallery.

For example, after the first image has been removed from the gallery above, it's HTML code should look like this:
```
<div class="image"> 
	<img src="https://goo.gl/d2JncW" alt="Second"> 
	<button class="remove">X</button> 
</div>
```
4. Closures

Fix the bugs in the registerHandlers function. An alert should display anchor's zero-based index within a document instead of following the link.

For example, in the document below, the alert should display "2" when Google anchor is clicked since it is the third anchor element in the document and its zero-based index is 2.

```
<body>
  In my life, I used the following web search engines:<br/>
  <a href="//www.yahoo.com">Yahoo!</a><br/>
  <a href="//www.altavista.com">AltaVista</a><br/>
  <a href="//www.google.com">Google</a><br/>
</body>
```

5. Avatar

Every user on your website has an image avatar that is displayed when they post a comment. You want to style these images differently from other images on your site. Add a CSS class named avatar that fulfils the following requirements:

    1. The avatar's border is rounded, so that it appears as a circle.
    2. The avatar's width and height are both 150px.
    3. The avatar has a solid border, has a width of 2px, and be colored gray.

For example, the avatar in the template should look like:

![Download it from https://www.testdome.com/files/resources/12362/554e82a4-b09e-4186-80c1-135f718f66c9.png](https://www.testdome.com/files/resources/12362/554e82a4-b09e-4186-80c1-135f718f66c9.png)


6. Inspector

Fix the bugs in the following HTML code.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Company page</title>
  </head>
  <body>
    <paragraph>Welcome! Here you can find the following things:</paragraph>
    <ol>
      <em><li><a href="#logo">Company's logo</a></li></em>
      <li><a href="#employees">List of employees</a></li>
    </ol>

    <h1>Company's logo
    <paragraph>Company uses the following logos:</paragraph>
    <ul>
      <li>New logo:</li><img source="new_logo.gif"/>
      <li>Old logo:</li><img source="old_logo.gif"/>
    </ul>

    <h1>List of employees
    <thead>
      <th>First name</th>
      <th>Last name</th>
    </thead>
    <table>
      <tr>
        <td>Mary</td>
        <td>Williams</td>
      </tr>
      <tr>
        <td>James</td>
        <td>Smith</td>
      </tr>
    </table>
  </body>
</html>
```

7. Semantics

Update the website's HTML, without using JavaScript or CSS, to make use of semantic elements so that:

  * The classless outer div element is replaced with a more appropriate element.
  * The divs with the image and caption classes are replaced with self-contained content elements.
  * The divs with the lorem-ipsum and description classes are replaced with elements, so that by default only the contents of the description element are shown. When the contents of the description element are clicked, the visibility of the rest of the lorem-ipsum element is toggled.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Semantics</title>
  </head>
  <body>
    <div>
      <h1>Lorem Ipsum</h1>
      
      <div class="image">
        <img src="https://goo.gl/zF9eky" alt="Lorem Ipsum">
        <div class="caption">Lorem Ipsum</div>
      </div>
      
      <div class="lorem-ipsum">
        <div class="description">Lorem ipsum dolor sit amet, consectetur adipiscing elit...</div>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
          Curabitur vitae hendrerit mauris. Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
          Mauris lacinia scelerisque nibh nec gravida. 
          Duis malesuada nec nibh sit amet pulvinar. 
          Phasellus congue porttitor arcu, ut suscipit nibh aliquam vel. 
          Nunc arcu lectus, egestas ut sem ac, euismod porttitor eros. 
          Phasellus tincidunt consequat pharetra. Maecenas sodales purus at nulla finibus dapibus. 
          Nullam varius at nisl vel euismod. Fusce aliquet ligula non tempor fermentum. 
          Nam fermentum posuere mauris, quis aliquam nibh dictum sed.</p>
      </div>
    </div>
  </body>
</html>
```

8. Food Ranking

A website needs a list where users can rank their favorite foods. Write the setup function, which should register click handlers on all Up! and Down! buttons. The Up! button should move the list item one place up in the list, while Down! button should move the list item one place down in the list.

For example, consider this code:
```
document.body.innerHTML = `<ol> 
  <li><button>Up!</button>Taco<button>Down!</button></li>
  <li><button>Up!</button>Pizza<button>Down!</button></li>
  <li><button>Up!</button>Eggs<button>Down!</button></li>
  </ol>`; 
setup();
```

If the button Up! button in Pizza list item is clicked, Pizza should be the first item in the list, while Taco should be the second item.
