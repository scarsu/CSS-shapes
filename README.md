# CSS-shapes
原生CSS实现各种形状

## split table header

<div class="split-header">
  <div class="right"></div>
  <div class="left"></div>
</div>

<style>
.split-header{
  width:200px;
  height:100px;
  background:#fff;
  position:relative;
}
.split-header .right{
  width:0;
  height:0;
  border-right:200px solid red;
  border-bottom:100px solid transparent;
}
.split-header .right:before{
  content:'column-right';
  position:absolute;
  right:0;
  top:30px;
}
.split-header .left{
  width:0;
  height:0;
  border-left:200px solid red;
  border-top:100px solid transparent;
  margin-top: -99px;
}
.split-header .left:before{
  content:'column-left';
  position:absolute;
  left:0;
  bottom:30px;
}
</style>

```html
<div class="split-header">
  <div class="right"></div>
  <div class="left"></div>
</div>
<style>
.split-header{
  width:200px;
  height:100px;
  background:#fff;
  position:relative;
}
.split-header .right{
  width:0;
  height:0;
  border-right:200px solid red;
  border-bottom:100px solid transparent;
}
.split-header .right:before{
  content:'column-right';
  position:absolute;
  right:0;
  top:30px;
}
.split-header .left{
  width:0;
  height:0;
  border-left:200px solid red;
  border-top:100px solid transparent;
  margin-top: -99px;
}
.split-header .left:before{
  content:'column-left';
  position:absolute;
  left:0;
  bottom:30px;
}
</style>
```

