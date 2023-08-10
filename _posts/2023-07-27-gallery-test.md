---
layout: gallery
title: "Gallery test"
date: 2023-07-27
categories:
---

<style>
p {text-align: center;}
</style>

<audio id="audio_01" src="/site/assets/audio/audio_cindyJulaton.mp3"></audio>
<audio id="audio_02" src="/site/assets/audio/audio_joanneHall.mp3"></audio>
<audio id="audio_03" src="/site/assets/audio/audio_olivierGutknecht.mp3"></audio>

<div class="main-carousel" data-flickity='{ "autoPlay": true, "wrapAround": true, "fade": true, "prevNextButtons": false }'>
  <div class="carousel-cell">
     <img id="img_01" src="/site/assets/img/img_cindyJulaton_present.jpg" onmouseover="playAudio_01()" onmouseout="pauseAudio_01()"/>
     <p>Cindy Julaton</p>
  </div>
  <div class="carousel-cell">
     <img id="img_02" src="/site/assets/img/img_joanneHall_present.jpg" onmouseover="playAudio_02()" onmouseout="pauseAudio_02()"/>
     <p>Joanne Paige Hall</p>
  </div>
  <div class="carousel-cell">
     <img id="img_03" src="/site/assets/img/img_olivierGutknecht_present.jpg" onmouseover="playAudio_03()" onmouseout="pauseAudio_03()"/>
     <p>Olivier Gutknecht</p>
  </div>
</div>

<script>
  var audio_01 = document.getElementById("audio_01");
  var audio_02 = document.getElementById("audio_02");
  var audio_03 = document.getElementById("audio_03");

  var img_01 = document.getElementById("img_01");
  var img_02 = document.getElementById("img_02");
  var img_03 = document.getElementById("img_03");

  function playAudio_01() {
    audio_01.play();
    img_01.src = "/site/assets/img/img_cindyJulaton_present_HOVER.png";
  }

  function playAudio_02() {
    audio_02.play();
    img_02.src = "/site/assets/img/img_joanneHall_present_HOVER.png";
  }

  function playAudio_03() {
    audio_03.play();
    img_03.src = "/site/assets/img/img_olivierGutknecht_present_HOVER.png";
  }

  function pauseAudio_01() {
    audio_01.pause();
    img_01.src = "/site/assets/img/img_cindyJulaton_present.jpg";
  }

  function pauseAudio_02() {
    audio_02.pause();
    img_02.src = "/site/assets/img/img_joanneHall_present.jpg";
  }

  function pauseAudio_03() {
    audio_03.pause();
    img_03.src = "/site/assets/img/img_olivierGutknecht_present.jpg";
  }

</script>
  
