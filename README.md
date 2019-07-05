### slidesJs
---

https://slidesjs.com/

https://github.com/nathansearles/Slides

```js
$(function(){
  $("#slides").slidesjs({
    width: 940,
    height: 528
  });
});

(function() {
  
  (function($, window, document) {
    var Plugin, defaults, pluginName;
    pluginName = "slidesjs";
    defaults = {
      width: 940,
      height: 528,
      start: 1,
      navigation: {
        active: true,
        effect: "slide"
      },
      pagination: {
        active: true,
        effect: "slide"
      },
      play: {
        active: false,
        effect: "slide",
        interval: 5000,
        auto: false,
        swap: true,
        pauseOnHover: false,
        restartDelay: 2500
      },
      effect: {},
      callback: {}
    };
    Plugin = (function() {
      
      function Plugin(element, options) {
        this.element = element;
        this.options = $.extend(true, {}, defaults, options);
        this._defaults = defaults;
        this._name = pluginName;
        this.init();
      }
      
      return Pluign;
      
    })();
    Plugin.prototype.init = function() {
      var $element, nextButton, pagination, playButton, prevButton, stopButton,
        _this = this;
      $element = $(this.element);
      this.data = $.data(this);
    }
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
