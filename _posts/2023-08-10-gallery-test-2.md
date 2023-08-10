---
layout: gallery
title: "Gallery test 2"
date: 2023-08-10
categories:
---

<style>
p {text-align: center;}

.galleryImage {
    width: 30%;
    height: auto;
    min-width: 300px;
}

.galleryDiv {
    width: 100%;
    margin-left: auto;
    margin-right: auto;
}

.text {
    width: 30%;
    min-width: 300px;
}
</style>
<div class="text">
A second prototype of the gallery featuring randomly ordered images and their respective text when hovered. Audio-on-hover has been removed. Refresh the page to get a new random ordering.
</div>
<script type="text/javascript">
    array_img = new Array();
    array_img[0] = "/site/assets/img/img_cindyJulaton_present.jpg";
    array_img[1] = "/site/assets/img/img_joanneHall_present.jpg";
    array_img[2] = "/site/assets/img/img_olivierGutknecht_present.jpg";

function getRandomImage(a, b, c) {
    var num = Math.floor( Math.random() * array_img.length);
    var img = array_img[num];
    document.getElementById("img_0" + a).src = img;
    array_img.splice(num, 1);
    var num = Math.floor( Math.random() * array_img.length);
    var img = array_img[num];
    document.getElementById("img_0" + b).src = img;
    array_img.splice(num, 1);
    var num = Math.floor( Math.random() * array_img.length);
    var img = array_img[num];
    document.getElementById("img_0" + c).src = img; 
}
</script>
<div>
  <div class="galleryDiv">
     <img id="img_01" src="" class="galleryImage" onmouseover="mouseON_01()" onmouseout="mouseOFF_01()"/> 
     <img id="img_02" src="" class="galleryImage" onmouseover="mouseON_02()" onmouseout="mouseOFF_02()"/>
     <img id="img_03" src="" class="galleryImage" onmouseover="mouseON_03()" onmouseout="mouseOFF_03()"/>
  </div>
</div>
<script>

  var img_01 = document.getElementById("img_01");
  var img_02 = document.getElementById("img_02");
  var img_03 = document.getElementById("img_03");

  function mouseON_01() {
    img_01.src = img_01.src.replace(/(.jpg)/, "_HOVER.png");
  }

  function mouseON_02() {
    img_02.src = img_02.src.replace(/(.jpg)/, "_HOVER.png");
  }

  function mouseON_03() {
    img_03.src = img_03.src.replace(/(.jpg)/, "_HOVER.png");
  }

  function mouseOFF_01() {
    img_01.src = img_01.src.replace(/(_HOVER.png)/, ".jpg");
  }

  function mouseOFF_02() {
    img_02.src = img_02.src.replace(/(_HOVER.png)/, ".jpg");
  }

  function mouseOFF_03() {
    img_03.src = img_03.src.replace(/(_HOVER.png)/, ".jpg");
  }

</script>

<body onload="getRandomImage(1, 2, 3)"></body>