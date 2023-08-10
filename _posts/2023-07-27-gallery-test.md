---
layout: gallery
title: "Gallery test"
date: 2023-07-27
categories:
---

<style>
p {text-align: center;}
</style>

<script type="text/javascript">
    array_img = new Array();
    array_img[0] = "/site/assets/img/img_cindyJulaton_present.jpg""
    array_img[1] = "/site/assets/img/img_joanneHall_present.jpg"
    array_img[2] = "/site/assets/img/img_olivierGutknecht_present.jpg"

function getRandomImage(element) {
    var num = Math.floor( Math.random() * array_img.length);
    var img = array_img[num];
    document.getElementById("img" + element).src = img;
}
</script>

<body onload="getRandomImage('_01')"
    onload="getRandomImage('_02')"
    onload="getRandomImage('_03')">


<div class="main-carousel" data-flickity='{ "autoPlay": true, "wrapAround": true, "fade": true, "prevNextButtons": false }'>
  <div class="carousel-cell">
     <img id="img_01" src="" onmouseover="mouseON_01()" onmouseout="mouseOFF_01()"/>
     <p>Cindy Julaton</p>
  </div>
  <div class="carousel-cell">
     <img id="img_02" src="" onmouseover="mouseON_02()" onmouseout="mouseOFF_02()"/>
     <p>Joanne Paige Hall</p>
  </div>
  <div class="carousel-cell">
     <img id="img_03" src="" onmouseover="mouseON_03()" onmouseout="mouseOFF_03()"/>
     <p>Olivier Gutknecht</p>
  </div>
</div>

<script>

  var img_01 = document.getElementById("img_01");
  var img_02 = document.getElementById("img_02");
  var img_03 = document.getElementById("img_03");

  var img_01_init = img_01.src;
  var img_02_init = img_02.src;
  var img_03_init = img_03.src;

  function mouseON_01() {
    img_01.src = img_01_init + "_HOVER";
  }

  function mouseON_02() {
    img_02.src = img_02_init + "_HOVER";
  }

  function mouseON_03() {
    img_03.src = img_03_init + "_HOVER";
  }

  function mouseOFF_01() {
    img_01.src = img_01_init;
  }

  function mouseOFF_02() {
    img_02.src = img_02_init;
  }

  function mouseOFF_03() {
    img_03.src = img_03_init;
  }

</script>
</body>  
