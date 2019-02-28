# sub-menu opacity

HTML
```html
<ul class="top-menu">
  <li><a href="#">Home</a></li>
  <li><a href="#">Work</a></li>
  <li><a href="#">About<i class="fa fa-angle-down"></i></a>
    <ul class="sub-menu">
      <li><a href="">Item 1</a></li>
      <li><a href="">Item 2</a></li>
    </ul>
  </li>
  <li><a href="#">Blog</a></li>
  <li><a href="#">Contact</a></li>
</ul>
```

CSS
```css
li {position: relative;display: inline-block;margin-right: 20px;}
.sub-menu {
  position: absolute;
  top: 100%;
  z-index: 10;
  background: #FFAB51;
  padding: 0;
  visibility: hidden;
  opacity: 0;
  transition: .3s;
}
ul li:hover .sub-menu {
  visibility: visible;
  opacity: 1;
}
```

# sub-menu transform

HTML
```html
<ul class="top-menu">
  <li><a href="#">Home</a></li>
  <li><a href="#">Work</a></li>
  <li><a href="#">About<i class="fa fa-angle-down"></i></a>
    <ul class="sub-menu">
      <li><a href="">Item 1</a></li>
      <li><a href="">Item 2</a></li>
    </ul>
  </li>
  <li><a href="#">Blog</a></li>
  <li><a href="#">Contact</a></li>
</ul>
```

CSS
```css
li {position: relative;display: inline-block;margin-right: 20px;}
.sub-menu {
  position: absolute;
  top: 100%;
  z-index: 10;
  -webkit-transition: 0.5s ease-in-out;
  -moz-transition: 0.5s ease-in-out;
  -o-transition: 0.5s ease-in-out;
  transition: 0.5s ease-in-out;
  -webkit-transform: scaleY(0);
  -ms-transform: scaleY(0);
  transform: scaleY(0);
  -webkit-transform-origin: 0 0;
  -ms-transform-origin: 0 0;
  transform-origin: 0 0;
  background: #FFAB51;
  padding: 0;
}
ul li:hover .sub-menu {
  -webkit-transform: scaleY(1);
  -ms-transform: scaleY(1);
  transform: scaleY(1);
}
```
