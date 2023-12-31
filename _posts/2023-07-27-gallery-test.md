---
layout: gallery
title: "Gallery test"
date: 2023-07-27
categories:
---

<style>
p {text-align: center;}

.main-carousel {
    min-width: 500px;
    width: 50%;
    margin-left: auto;
    margin-right: auto;
}
</style>

This is a technical test on a rotating carousel. It rotates automatically given enough time, and can also be 'flicked' through with the user's cursor or finger in the case of mobile. It can also be navigated using the dots along the bottom. Quotes on hover definitely need a different font, but the idea might be worth pursuing?

<div class="main-carousel" data-flickity='{ "autoPlay": true, "wrapAround": true, "fade": true, "prevNextButtons": false }'>
  <div class="carousel-cell">
     <img id="img_01" src="/site/assets/img/img_cindyJulaton_present.jpg" onmouseover="mouseON_01()" onmouseout="mouseOFF_01()"/>
     <p>Cindy Julaton</p>
  </div>
  <div class="carousel-cell">
     <img id="img_02" src="/site/assets/img/img_joanneHall_present.jpg" onmouseover="mouseON_02()" onmouseout="mouseOFF_02()"/>
     <p>Joanne Paige Hall</p>
  </div>
  <div class="carousel-cell">
     <img id="img_03" src="/site/assets/img/img_olivierGutknecht_present.jpg" onmouseover="mouseON_03()" onmouseout="mouseOFF_03()"/>
     <p>Olivier Gutknecht</p>
  </div>
</div>

<script>

  var img_01 = document.getElementById("img_01");
  var img_02 = document.getElementById("img_02");
  var img_03 = document.getElementById("img_03");

  function mouseON_01() {
    img_01.src = "/site/assets/img/img_cindyJulaton_present_HOVER.png";
  }

  function mouseON_02() {
    img_02.src = "/site/assets/img/img_joanneHall_present_HOVER.png";
  }

  function mouseON_03() {
    img_03.src = "/site/assets/img/img_olivierGutknecht_present_HOVER.png";
  }

  function mouseOFF_01() {
    img_01.src = "/site/assets/img/img_cindyJulaton_present.jpg";
  }

  function mouseOFF_02() {
    img_02.src = "/site/assets/img/img_joanneHall_present.jpg";
  }

  function mouseOFF_03() {
    img_03.src = "/site/assets/img/img_olivierGutknecht_present.jpg";
  }

</script> 
