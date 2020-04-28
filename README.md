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

```javascript
//.form-group and .form-control 
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

```javascript
<nav class="navbar navbar-default"> //navbar
<div class="container">  //putting all the items in container
  <div class="navbar-header"> //first item 
    <a href="#" class="navbar-header">Koffee</a>
  </div>
  <ul class="nav navbar-nav"> //items
    <li><a href="#">About</a></li>
    <li><a href="#">Contact</a></li>
  </ul>
  <ul class="nav navbar-nav navbar-right"> //items to the left
    <li><a href="#">Sign In</a></li>
    <li><a href="#">Sign Up</a></li>
  </ul>
</div>
</nav>
```

To implement actions/features include jquery cdn first and then the bootstrap javascript cdn because it relies on jquery. (This already done in <em>There are 2 ways to use Bootstrap</em>

```javascript
// including a hamburger
// hiding our items to a humber in mobile version
<nav class="navbar navbar-default"> //navbar
<div class="container">  //putting all the items in container
  <div class="navbar-header"> //first item 
    // implementing the hamburger icon, must be put before the navbar header
    // pay attention to data-target attribute, the value we set to it is the items we're going to collapse 
    <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target-"#bs-nav-demo" aria-        expanded="false">
      // each span is just drawing the bars in our icon
      <span class="sr-only">Toggle Navigation</span>
      <span class="icon-bar"></span>
      <span class="icon-bar"></span>
      <span class="icon-bar"></span>
    </button>
    <a href="#" class="navbar-header">Koffee</a>
  </div>
//collapsible items start here
<div class="collapse navbar-collapse" id="bs-nav-demo"> //whatever we put inside here will be collapsible by the burger, this is targetted by our burger component/icon, see id
  // we're putting our items here
  <ul class="nav navbar-nav"> //items
    <li><a href="#">About</a></li>
    <li><a href="#">Contact</a></li>
  </ul>
  <ul class="nav navbar-nav navbar-right"> //items to the left
    <li><a href="#">Sign In</a></li>
    <li><a href="#">Sign Up</a></li>
  </ul>
</div>
```



