---
layout: default
title: Home
---
<!-- 👇 STEP 1: Paste banner slider code here -->
<div class="banner-slider">
  <div class="slide fade">
    <img src="/assets/images/banner1.jpg" />
  </div>
  <div class="slide fade">
    <img src="/assets/images/banner2.jpg" />
  </div>
  <div class="slide fade">
    <img src="/assets/images/banner3.jpg" />
  </div>
</div>

<style>
.banner-slider {
  max-width: 100%;
  height: 320px;
  position: relative;
  overflow: hidden;
}
.slide {
  display: none;
  position: absolute;
  width: 100%;
  height: 100%;
}
.slide img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.fade {
  animation: fadeEffect 1s;
}
@keyframes fadeEffect {
  from { opacity: 0.4 }
  to { opacity: 1 }
}
</style>

<script>
let slideIndex = 0;
showSlides();
function showSlides() {
  const slides = document.getElementsByClassName("slide");
  for (let i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";
  }
  slideIndex++;
  if (slideIndex > slides.length) {slideIndex = 1}
  slides[slideIndex - 1].style.display = "block";
  setTimeout(showSlides, 3000);
}
</script>

<!-- 👇 STEP 2: Existing hero content below -->
<h1 style="text-align: center;">Welcome to Quiz Wallah</h1>
<p style="text-align: center;">India's Smartest MCQ Practice App...</p>

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


<div style="background-color: white; padding: 2rem 1rem;">
  <h2 style="text-align: center;">Why Choose Quiz Wallah?</h2>
<ul style="max-width: 700px; margin: auto; font-size: 1rem;">
  <li>✅ Daily MCQ assignments with instant results</li>
  <li>🔁 Practice old assignments anytime, as many times</li>
  <li>👪 Parent dashboard to track child’s performance</li>
  <li>🏫 School-wise reports generated automatically</li>
  <li>🎯 Perfect screen-time use: productive, educational, fun!</li>
</ul>


<div style="background-color: #f0fbff; padding: 2rem 1rem;">
  <h3 style="text-align: center;">App Preview</h3>
  <p style="text-align: center; margin-top: 1rem; font-style: italic; color: #555;">
  More features & updates added regularly – based on student and school feedback.
</p>

  <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 20px; padding: 1rem;">
    <img src="/assets/images/screenshot1.png" style="width: 200px; border-radius: 8px;" />
   <img src="/assets/images/screenshot2.png" alt="Screenshot 2" style="width: 200px; border-radius: 8px;" />
  <img src="/assets/images/screenshot3.png" alt="Screenshot 3" style="width: 200px; border-radius: 8px;" />
  <img src="/assets/images/screenshot4.png" alt="Screenshot 4" style="width: 200px; border-radius: 8px;" />
  <img src="/assets/images/screenshot5.png" alt="Screenshot 5" style="width: 200px; border-radius: 8px;" />
  <img src="/assets/images/screenshot6.png" alt="Screenshot 6" style="width: 200px; border-radius: 8px;" />
  </div>
</div>


<hr style="margin: 2rem 0;" />

