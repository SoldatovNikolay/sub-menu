# sub-menu opacity

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

 & transform
