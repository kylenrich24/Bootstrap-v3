# Bootstrap-v3
<img src="https://blog.templatetoaster.com/wp-content/uploads/2019/09/What-is-Bootstrap-Facebook.png" height="500" width="1000">
<p>Bootstrap is an HTML, CSS and JS framework for developing responsive, mobile-first projects on the web.</p>
<p>DOCS: https://getbootstrap.com/docs/4.3/components/alerts/</p>
<br>
<hr>
<p>There are 2 ways to use Bootsrap:</p>
<ul>
<li>Download the files and it to your application</li>
  <ol>
    <li>Download the files https://getbootstrap.com/docs/4.3/getting-started/download/</li>
    <li>We need <em>bootstrap.css</em> or <em>bootstrap.min.css</em> from <em>/css/css/bootstrap.css</em></li>
    <li>Copy and paste this to the same directory where your app is in</li>
    <li>Link using a stylesheet link tag</li>
  </ol>
<li>Link CDN</li>
  <ol>
    <li>Link the CSS cdn into the head of your HTML doc </li>
     <li>Link the JS cdn into the script before closing the body tag</li>
</ul>
    </ol>
  <br>
 
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
   <br>
   <pre><code>
<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM" crossorigin="anonymous"></script>
   </code></pre>
<br><br<
<p><strong>We can now start using Bootstrap components by adding classes to our elements</strong><p>
<hr>
<br>
<h3>Buttons</h3>
<p>We can use an <em>a</em>, <em>button</em> and <em>input</em> tag and apply the class:</p>
<br>


```javascript
<a class="btn btn-danger btn-lg"></a>
```


    
<br>
<br>
<h3>Jumbotron</h3>
<img src="https://css3menu.com/web-design/data/upload/2017/04/example-jumb.jpg" height=400px width=700px>
<p>Jumbotron takes up 100% of whatever container it's inside of.</p>
<br>


```javascript
<div class="container"> //we put the jumbotron in a container that has auto margin to center
  <div class="jumbotron">
    //everything we put here will be in the jumbotron
    <h1>Hello There</h1>
    <button class="btn btn-success bn-lg">Click Me</button>
  </div>
</div>

```

<br>
<br>
<h3>Forms</h3>

```html
//pay attention to .form-group and .form-control classes
<form>
  <div class="form-group"> //we put every block in a form-group
   <label for="id">Email</label>
   <input type="email" class="form-control" id="id">
  </div>
  <div class="form-group"> //we put every block in a form-group
    <label for="id">Password</label>
    <input type="password" class="form-control" id="id">
  </div>
</form>

// in-line form 
<form class="in-line">  //gotta add this 
  <div class="form-group"> //we put every block in a form-group
    <label for="id">Email</label>
    <input type="email" class="form-control" id="id">
  </div>
  <div class="form-group"> //we put every block in a form-group
    <label for="id">Password</label>
    <input type="password" class="form-control" id="id">
  </div>
</form>
```


<br>
<br>
<h3>Navbar</h3>

```html
 <nav class="navbar navbar-expand-lg navbar-light bg-light"> // makes our navbar, navbar items stack except lg
  <div class="container">  // makes sure all our items are in a center margin
    <a class="navbar-brand" href="#">Navbar</a>  // our main item
      <div class="navbar-collapse">  // everything in here will be our items
        <div class="navbar-nav">  // layouts our item properly
          <a class="nav-item nav-link" href="#">Home</a>  //item
          <a class="nav-item nav-link" href="#">About</a> //item
        </div>
      </div>
      <div class="navbar-nav">  //layouts our item properly; not inside navbar-collapse; it will stick to the left side
        <a class="nav-item nav-link" href="#">Sign In</a> //item
        <a class="nav-item nav-link" href="#">Sign Out</a>  //item
      </div>
  </div>
 </nav>
```

<br>
<br>

<img src="https://www.script-tutorials.com/wp-content/uploads/2015/01/navbar3-700x357.jpg" height=200px width=500px>

<br>

To implement actions/features include jquery cdn first and then the bootstrap javascript cdn because it relies on jquery. (This already done in <em>There are 2 ways to use Bootstrap</em>

```html
// including a hamburger
// hiding our items to a hamburger in mobile version

<nav class="navbar navbar-expand-lg navbar-dark" style="background-color: red;"> //NAVBAR; stacks except in lg; white text(navbar-dark)
  <div class="container"> // putting all our items in a container; has auto margin to center
    <a class="navbar-brand" href="#">Navbar</a> // MAIN ITEM
    // HAMBURGER ICON THAT TARGETS OUR ITEM TO COLLAPSE
    <button
      class="navbar-toggler"
      type="button
      data-toggle="collapse"
      data-target="#navbarSupportedContent"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    
    <div class="collapse navbar-collapse" id="navbarSupportedContent"> // pur items; items collapsible to hamburger
      <ul class="navbar-nav mr-auto"> //layouts our items properly to stack to the left; our first set of items
        <li>
          <a class="nav-link" href="#">Home</a>  //ITEM
        </li>
        <li>
          <a class="nav-link" href="#">Link</a> //ITEM
        </li>
      </ul>
      <ul class="navbar-nav navbar-right"> //layouts our items to the right; our second set of items
        <li>
          <a class="nav-link" href="#">Sign In</a>  //ITEM
        </li>
        <li>
          <a class="nav-link" href="#">Sign Out</a> //ITEM
        </li>
      </ul>
    </div>
  </div>
</nav>
```

<br>
<br>
<hr>
<br>
<br>

<h2>The Grid System</h2>
<p>Some consider that most people use Bootstrap for the Grid System. It acts like a skeleton of our entire application. It enables us to easily add structure and layout to our application. For instance we can say that we want our application to take up 100% of our screen, then we can also say that we want our components to take 25% of the screen and take 50% when we hit the mobile size.</p>
<p>DOCS: https://getbootstrap.com/docs/3.4/css/#grid</p>
<br>
<p><em>12</em>. Every container in bootstrap can be divided into 12 different columns. Using the Grid System we can pick how many of those 12 units each of our elements should take up.  </p>
<br>

<img src="https://miro.medium.com/max/2342/1*6frm0pq5VjPcc71EqH7cKw.png" height="300" width="550"/>

<br>

<p>Every time we want to use a Bootstrap grid, we use a container.</p>


```javascript
// Using a 50/50 Grid System
<div class="container> //this is the same container that we have been using. It has auto margin to center
  <div class="row">
    <div class="col-lg-6">  //We're using 6 out of 12 - 50%
      
    </div>  
    <div class="col-lg-6">  //We're using 6 out of 12 - 50%
    
    </div>  
  </div>
</div>
```


```javascript
// Using a different layout 2/8/2 
<div class="container> //this is the same container that we have been using. It has auto margin to center
  <div class="row">
    <div class="col-lg-2">  //We're using 2 out of 12 in this container
      
    </div>  
    <div class="col-lg-8">  //We're using 8 out of 12 in this container
      
    </div> 
    <div class="col-lg-2">  //We're using 2 out of 12 in this container
    
    </div>  
  </div>
</div>
// We can designate these 12 units however we want
```

<h3>Making the Grid Responsive</h3>
<p><strong>col-lg-6.</strong> There are 4 sizes we can use. We can specify layout/ratios in each of these sizes. We have xs, sm, md, lg. </p>


```javascript
// making our layout responsive 
// using 4 columns (3/12 units each container) in md to lg and 6 units (2 columns) in sm

<div class="container> //this is the same container that we have been using. It has auto margin to center
  <div class="row">
    <div class="col-md-3 col-sm-6">  //6/12 units in sm; it will take up 50% of the tablet size
      
    </div>  
    
    <div class="col-md-3 col-sm-6">  //50% in sm
      
    </div> 
    
    <div class="col-md-3 col-sm-6">  // this will stack below because it has to take up 50% too
    
    </div>  
    
    <div class="col-md-3 col-sm-6">  //50% in sm
    
    </div>  
  </div>
</div>
```
<br>
We can also nest grids. This means dividing our container further to another grid.

```javascript
<div class="col-md-3 col-sm-6">  //6/12 units in sm; it will take up 50% of the tablet size
  <div class="row"> //nested grid
    <div class="col-lg-6">  //50% column
      
    </div>  
    <div class="col-lg-6">  // another column
      
    </div>  
</div>  
```
