---
title: A Semi-famous Chinese-Korean Restaurant in Incheon
description: Black bean noodles and jjam-bbong
date: 2020-06-17
tags:
  - korean-chinese-food
layout: layouts/post.njk
---
There are hundreds, if not thousands, of Koreanized Chinese restaurants in Korea. Koreans love jja-jang-myun (noodles with black bean sauce) and jjam-bbong (spicy seafood soup) as much as Americans love burgers and hotdogs.

At bare minimum, you'll find these 3 entrees on the menu:

- fried pork with sweet sauce (tang-soo-yuk)
- jja-jang-myun
- jjam-bbong

It's not possible to rank all the Sino-Korean establishments in Korea. There's too many and very little variation. (You can say that about almost anything in Korea.) Some of these stand out due to how old they are or offer a unique menu option.

If you find yourself in Incheon, there's a place called "Yeon-Joong-Ban-Jeom", near Seokbawi Market Station (Exit 2). It's been around, having opened in 1956. (That's just 3 years after the end of the Korean War!)

<!-- Add images to masonry layout -->
<div class="masonry">
	<div class="item">
		<img src="../../img/f1.jpeg" style="width:100%" onclick="openModal();currentSlide(1)" class="hover-shadow cursor" alt="Yeon-Joong-Ban-Jeom">
	</div>
	<div class="item">
		<img src="../../img/f2.jpeg" style="width:100%" onclick="openModal();currentSlide(2)" class="hover-shadow cursor" alt="noodles">
	</div>
	<div class="item">
		<img src="../../img/f3.jpeg" style="width:100%" onclick="openModal();currentSlide(3)" class="hover-shadow cursor" alt="spicy noodles">
	</div>
	<div class="item">
		<img src="../../img/f4.jpeg" style="width:100%" onclick="openModal();currentSlide(4)" class="hover-shadow cursor" alt="jja jang myeon" />
	</div>
	<div class="item">
		<img src="../../img/f5.jpeg" style="width:100%" onclick="openModal();currentSlide(5)" class="hover-shadow cursor" alt="good food" />
	</div>
	<div class="item">
		<img src="../../img/f6.jpeg" style="width:100%" onclick="openModal();currentSlide(6)" class="hover-shadow cursor" alt="dark noodle" />
	</div>
	<div class="item">
		<img src="../../img/f7.jpeg" style="width:100%" onclick="openModal();currentSlide(7)" class="hover-shadow cursor" alt="hello china" />
	</div>
	<div class="item">
		<img src="../../img/f8.jpeg" style="width:100%" onclick="openModal();currentSlide(8)" class="hover-shadow cursor" alt="myeon" />
	</div>
	<div class="item">
		<img src="../../img/f9.jpeg" style="width:100%" onclick="openModal();currentSlide(9)" class="hover-shadow cursor" alt="random" />
	</div>
</div>
<div id="myModal" class="modal">
  <span class="close cursor" onclick="closeModal()">&times;</span>
  <div class="modal-content">
    <div class="mySlides">
      <div class="numbertext">1 / 9</div>
      <img src="../../img/f1.jpeg" style="width:100%">
    </div>
    <div class="mySlides">
      <div class="numbertext">2 / 9</div>
      <img src="../../img/f2.jpeg" style="width:100%">
    </div>
    <div class="mySlides">
      <div class="numbertext">3 / 9</div>
      <img src="../../img/f3.jpeg" style="width:100%">
    </div>
    <div class="mySlides">
      <div class="numbertext">4 / 9</div>
      <img src="../../img/f4.jpeg" style="width:100%">
    </div>
	<div class="mySlides">
      <div class="numbertext">5 / 9</div>
      <img src="../../img/f5.jpeg" style="width:100%">
    </div>
	<div class="mySlides">
      <div class="numbertext">6 / 9</div>
      <img src="../../img/f6.jpeg" style="width:100%">
    </div>
	<div class="mySlides">
      <div class="numbertext">7 / 9</div>
      <img src="../../img/f7.jpeg" style="width:100%">
    </div>
	<div class="mySlides">
      <div class="numbertext">8 / 9</div>
      <img src="../../img/f8.jpeg" style="width:100%">
    </div>
	<div class="mySlides">
      <div class="numbertext">9 / 9</div>
      <img src="../../img/f9.jpeg" style="width:100%">
    </div>
    <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
    <a class="next" onclick="plusSlides(1)">&#10095;</a>
    <div class="caption-container">
      <p id="caption"></p>
    </div>
    <div class="column">
      <img class="demo cursor" src="../../img/f1.jpeg" style="width:100%" onclick="currentSlide(1)" alt="Chinese food">
    </div>
    <div class="column">
      <img class="demo cursor" src="../../img/f2.jpeg" style="width:100%" onclick="currentSlide(2)" alt="spicy noodles">
    </div>
    <div class="column">
      <img class="demo cursor" src="../../img/f3.jpeg" style="width:100%" onclick="currentSlide(3)" alt="jja jang myeon">
    </div>
    <div class="column">
      <img class="demo cursor" src="../../img/f4.jpeg" style="width:100%" onclick="currentSlide(4)" alt="hot mustard">
    </div>
	<div class="column">
      <img class="demo cursor" src="../../img/f5.jpeg" style="width:100%" onclick="currentSlide(5)" alt="grub" />
    </div>
	<div class="column">
      <img class="demo cursor" src="../../img/f6.jpeg" style="width:100%" onclick="currentSlide(6)" alt="swefefwf" />
    </div>
	<div class="column">
      <img class="demo cursor" src="../../img/f7.jpeg" style="width:100%" onclick="currentSlide(7)" alt="beans" />
    </div>
	<div class="column">
      <img class="demo cursor" src="../../img/f8.jpeg" style="width:100%" onclick="currentSlide(8)" alt="saucy" />
    </div>
	<div class="column">
      <img class="demo cursor" src="../../img/f9.jpeg" style="width:100%" onclick="currentSlide(9)" alt="beans" />
    </div>
  </div>
</div>

<script>

function openModal() {
  document.getElementById("myModal").style.display = "block";
}

function closeModal() {
  document.getElementById("myModal").style.display = "none";
}

var slideIndex = 1;
showSlides(slideIndex);

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  var i;
  var slides = document.getElementsByClassName("mySlides");
  var dots = document.getElementsByClassName("demo");
  var captionText = document.getElementById("caption");
  if (n > slides.length) {slideIndex = 1}
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
      slides[i].style.display = "none";
  }
  for (i = 0; i < dots.length; i++) {
      dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";
  dots[slideIndex-1].className += " active";
  captionText.innerHTML = dots[slideIndex-1].alt;
}
</script>
