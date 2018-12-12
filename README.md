### slidesJs
---

https://slidesjs.com/

```js
$(function(){
  $("#slides").slidesjs({
    width: 940,
    height: 528
  });
});
```

```
<head>
  <style>
    #slides {
      display:none;
    }
  </style>
<script src="http://code.jquery.com/jquery-latest.min.js"></script>
<script src="jquery.slides.min.js"></script>
<script>
</scirpt>
</head>
<body>
  <div id="sides">
    <img src="http://placehold.it/940x528">
    <img src="http://placehold.it/940x528">
    <img src="http://placehold.it/940x528">
    <img src="http://placehold.it/940x528">
    <img src="http://placehold.it/940x528">
  </div>
</body>
```

```js
$(function(){
  $("#slides").slidesjs({
    width: 700,
    height: 393
  });
});

$(function(){
  $("#slides").slidesjs({
    start: 3
  });
});

$(function(){
  $("#slides").slidesjs({
    navigation: {
      active: true,
      effect: "slide"
    }
  });
});

$(function(){
  $("#slides").slidesjs({
    pagination: {
      active: true,
      effect: "slide"
    }
  });
});

$(function(){
  $("#slides").slidesjs({
    play: {
      active: true,
      effect: "slide",
      interval: 5000,
      auto: false,
      swap: false,
      pauseOnHover: false,
      restartDelay: 2500
    }
  });
});

$(function(){
  $("#slides").slidesjs({
    effect: {
      slides: {
        speed: 200
      },
      fade: {
        speed: 300,
        crossfadeL true
      }
    }
  });
});

$(function(){
  $("#slides").slidesjs({
    callback: {
      loaded: function(number){
      },
      start: function(number){
      },
      complete: function(number){
      }
    }
  });
});
```
