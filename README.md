jqListener
====

jQuery plugin to listen from twitter.

Continuously fetch content from Twitter and display them in a waterfall view.

![Preview screenshot](https://raw.github.com/zhangxin840/jqListener/master/screenShot.jpg)


Usage:
====

```
<!-- Add to header -->
<script src="http://code.jquery.com/jquery-latest.js"></script>
<script src="js/jqListener.min.js"></script>
<link rel="stylesheet" href="css/jqListener.min.css" />

<!-- Add to body -->
<div class="jqListener"></div>

//Start up jqListener
$(function() {
  $('.jqListener').jqListener({
        keyword : "apple",
        language : "en",
        maxNum : 6, //Max number of tweets the container can hold
        firstNum : 3, //Number of tweets of the first request
        animation : true,
        animationSpeed : 1500,
        fetchInterval : 2000
  });
});

//Search another keyword
$(".jqListener:first").changeListening("ipad");

```
