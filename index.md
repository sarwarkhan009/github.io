---
layout: default
title: Home
---

<!-- 👇 Clean Slider with sliding transition -->

<div class="fade-slider">
  <img class="fade-slide" src="/assets/images/banner1.png" alt="Banner 1">
  <img class="fade-slide" src="/assets/images/banner2.png" alt="Banner 2">
  <img class="fade-slide" src="/assets/images/banner3.png" alt="Banner 3">
  <img class="fade-slide" src="/assets/images/banner4.png" alt="Banner 4">
  <img class="fade-slide" src="/assets/images/banner5.png" alt="Banner 5">
</div>

<style>
.fade-slider {
  position: relative;
  width: 100%;
  height: 480px; /* banner height */
  overflow: hidden;
}

.fade-slide {
  position: absolute;
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center;
  opacity: 0;
  transition: opacity 1s ease-in-out;
}

.fade-slide.active {
  opacity: 1;
  z-index: 1;
}
</style>

<script>
let fadeIndex = 0;
const slides = document.getElementsByClassName('fade-slide');

function showFadeSlides() {
  for (let i = 0; i < slides.length; i++) {
    slides[i].classList.remove("active");
  }
  fadeIndex++;
  if (fadeIndex > slides.length) { fadeIndex = 1 }
  slides[fadeIndex - 1].classList.add("active");
  setTimeout(showFadeSlides, 4000); // 4 seconds per slide
}

showFadeSlides();
</script>


<!-- Hero Title and Tagline Section -->
<section style="text-align: center; padding: 2rem 1rem; background-color: #e3f2fd;">
  <h1 style="font-size: 2.2rem; font-weight: 700; text-shadow: 1px 1px 2px rgba(0,0,0,0.1); margin-bottom: 0.5rem;">
    Welcome to Quiz Wallah
  </h1>
  <p style="font-size: 1.2rem; color: #333;">
    India’s Smartest MCQ Practice App for Students of Class 1 to 10
  </p>
  <div style="margin-top: 1.5rem;">
    <a href="#"
       style="background-color: #28a745; color: white; padding: 14px 28px; font-size: 1.1rem;
              text-decoration: none; border-radius: 6px; font-weight: bold;
              box-shadow: 2px 2px 8px rgba(0,0,0,0.15); transition: all 0.2s ease;"
       onmouseover="this.style.backgroundColor='#218838'; this.style.transform='scale(1.05)'"
       onmouseout="this.style.backgroundColor='#28a745'; this.style.transform='scale(1)'">
      Get the App
    </a>
  </div>
</section>



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
