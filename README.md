### CSS-NOTES

#### Responsive Image
```css
.demo-img {display:flex;justify-content:center;} /* Center Image */
.demo-img img{width:100%;max-width:200px;} /* Responsive Image */
<div class="demo-img"><img src="demo.jpg"></div>
```
#### Responsive Tiles
```css
.tile-container {
 	display: flex;
 	flex-direction:row;
  padding:40px 0 60px 0;
 }
 
.tile-image {display:flex;justify-content:center;}
 .tile-image img{width:100%;max-width:330px;} 
.tile{
        flex:33%; /* Tile Width */
        margin:.5em;
        background:#fcfcfc;
        vertical-align:top;
        border: solid #eeeeee;
        border-width: 8px 0px 0.2em 0px;
        border-radius:5px 5px 0 0;
        border-top-color:#0e6021;
}
.tile-title{ font-weight: 600;font-size:1em; }
.tile-body {
        padding: .5em;
        text-align:left;
}
@media (max-width: 800px) {
  .tile-container { flex-direction: column; }
}

<div class="tile-container">
  <div class="tile">
    <span class="tile-image">
      <img src="">
    </span>
    <div class="tile-body">
      <div class="tile-title">Demo Title</div>
      <div class="tile-excerpt"><p>This is a demo summary...</p></div>
        <a rel="nofollow" class="external text" href="">Readmore</a>
    </div>
  </div>
</div>

```
