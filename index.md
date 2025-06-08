---
layout: default
title: Home
---

<!-- 👇 Clean Slider with sliding transition -->


<div class="slider">
  <div class="slides">
    <div class="slide"><img src="/assets/images/banner1.png" alt="Banner 1"></div>
    <div class="slide"><img src="/assets/images/banner2.png" alt="Banner 2"></div>
    <div class="slide"><img src="/assets/images/banner3.png" alt="Banner 3"></div>
    <div class="slide"><img src="/assets/images/banner4.png" alt="Banner 4"></div>
    <div class="slide"><img src="/assets/images/banner5.png" alt="Banner 5"></div>
  </div>
</div>

<style>
.slider {
  position: relative;
  width: 100%;
  max-width: 100%;
  height: auto;
  overflow: hidden;
}

.slides {
  display: flex;
  width: 500%;
  animation: slideShow 25s infinite;
}

.slide {
  flex: 0 0 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.slide img {
  width: 100%;
  max-height: 500px;
  height: auto;
  object-fit: contain;
  display: block;
}
@keyframes slideShow {
  0%   { transform: translateX(0%); }
  20%  { transform: translateX(0%); }
  25%  { transform: translateX(-100%); }
  45%  { transform: translateX(-100%); }
  50%  { transform: translateX(-200%); }
  70%  { transform: translateX(-200%); }
  75%  { transform: translateX(-300%); }
  95%  { transform: translateX(-300%); }
  100% { transform: translateX(-400%); }
}
</style>



<script>
let slidePos = 0;
const images = document.querySelectorAll(".slider-image");
const track = document.querySelector(".slider-track");

function showNextSlide() {
  slidePos = (slidePos + 1) % images.length;
  track.style.transform = `translateX(-${slidePos * 100}%)`;
}

setInterval(showNextSlide, 4000); // 4 seconds per slide
</script>


<!-- 👇 HERO SECTION -->
<h1 style="text-align: center; font-size: 2rem; text-shadow: 1px 1px 2px rgba(0,0,0,0.1);">
  Welcome to Quiz Wallah
</h1>

<p style="text-align: center; font-size: 1.1rem;">
  India's Smartest MCQ Practice App for Students of Class 1 to 10
</p>

<p style="text-align: center; margin-top: 1.5rem;">
  <a href="#"
     style="background-color: #28a745; color: white; padding: 16px 32px; font-size: 1.1rem;
            text-decoration: none; border-radius: 8px; font-weight: bold;
            box-shadow: 2px 2px 8px rgba(0,0,0,0.15);
            transition: all 0.2s ease;"
     onmouseover="this.style.backgroundColor='#218838'; this.style.transform='scale(1.05)';"
     onmouseout="this.style.backgroundColor='#28a745'; this.style.transform='scale(1)';">
    Get the App
  </a>
</p>


<!-- 👇 FEATURES SECTION -->
<div style="background-color: white; padding: 2rem 1rem;">
  <h2 style="text-align: center;">Why Choose Quiz Wallah?</h2>
  <ul style="max-width: 700px; margin: auto; font-size: 1rem;">
    <li>✅ Daily MCQ assignments with instant results</li>
    <li>🔁 Practice old assignments anytime, as many times</li>
    <li>👪 Parent dashboard to track child’s performance</li>
    <li>🏫 School-wise reports generated automatically</li>
    <li>🎯 Perfect screen-time use: productive, educational, fun!</li>
  </ul>
</div>


<!-- 👇 APP PREVIEW SECTION -->
<div style="background-color: #f0fbff; padding: 2rem 1rem;">
  <h3 style="text-align: center;">App Preview</h3>
  <p style="text-align: center; margin-top: 1rem; font-style: italic; color: #555;">
    More features & updates added regularly – based on student and school feedback.
  </p>

  <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 20px; padding: 1rem;">
    <img src="/assets/images/screenshot1.png" alt="Screenshot 1" style="width: 200px; border-radius: 8px;" />
    <img src="/assets/images/screenshot2.png" alt="Screenshot 2" style="width: 200px; border-radius: 8px;" />
    <img src="/assets/images/screenshot3.png" alt="Screenshot 3" style="width: 200px; border-radius: 8px;" />
    <img src="/assets/images/screenshot4.png" alt="Screenshot 4" style="width: 200px; border-radius: 8px;" />
    <img src="/assets/images/screenshot5.png" alt="Screenshot 5" style="width: 200px; border-radius: 8px;" />
    <img src="/assets/images/screenshot6.png" alt="Screenshot 6" style="width: 200px; border-radius: 8px;" />
  </div>
</div>

<hr style="margin: 2rem 0;" />
