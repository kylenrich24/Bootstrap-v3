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
<p>We can use an <em>a</em>, <em>button</em> and <em>input</em> tag and apply the class:<br>
  <em>btn  &nbsp;&nbsp; btn-success&nbsp;&nbsp; btn-xs &nbsp;&nbsp;active</em>
</p>
    
<br>
<br>
<h3>Jumbotron</h3>
<img src="https://css3menu.com/web-design/data/upload/2017/04/example-jumb.jpg" height=400px width=700px>
<p>Jumbotron takes up 100% of whatever container it's inside of.</p>
<br>
<code>
```jsx
  <div class="container> //we're putting the jumbotron in a container that has auto margin to center
    <div class=""jumbotron>
     //Whatever we put here will be inside of the jumbotron
     <h1>Hi There</h1>
     <button class="btn btn-success btn-lg">Learn More</button>
   </div>  
                                    </div>                                 
```
  
  
   
  
