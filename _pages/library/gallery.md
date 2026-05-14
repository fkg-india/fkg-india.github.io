---
title: "<p style='font-size: 0.8em;'>Gallery</p>"
layout: single
permalink: /library/gallery/
toc: false
sidebar:
  nav: sidebar
  sticky: true

header:
  height: "90vh"
  overlay_image: /assets/images/gallery/icpr-0.jpg
  caption: "IIT Kharagpur Kolkata Extension Centre, Kolkata (India) [Dec., 2024]"


bdbio24:
  - image_path: /assets/images/gallery/bdbio-1.jpg
    excerpt: "Big Data Algorithms for Biology (BDBio) Symposium hosted at Indian Institute of Science (IISc), Bangalore [May 2024]"

ashoka_expo24:
  - image_path: /assets/images/gallery/ashoka_expo-1.jpg
  - image_path: /assets/images/gallery/ashoka_expo-2.jpeg
    excerpt: "Centre Expo, Ashoka University [Dec., 2024]"
  - image_path: /assets/images/gallery/ashoka_expo-3.jpg

icpr2024:
  - image_path: /assets/images/gallery/icpr-1.jpg
  - image_path: /assets/images/gallery/icpr-4.jpg
    excerpt: "9th International Workshop on Multimedia Assisted Dietary Management (MADiMa) in conjunction with the 27th International Conference on Pattern Recognition (ICPR 2024), Kolkata (IN) [Dec. 2024]"
  - image_path: /assets/images/gallery/icpr-3.jpg

icpr_zoom2024:
  - image_path: /assets/images/gallery/icpr-2.png
    excerpt: "Zoom Meet with international food computing researchers, Kolkata/Hybrid [Dec. 2024]"

brf25:
  - image_path: /assets/images/gallery/brf-1.jpg
  - image_path: /assets/images/gallery/brf-2.jpg
    excerpt: "Building Resilient Futures: Data Skilling for Climate and Health, Ashoka University (IN) [Feb. 2025]"
  - image_path: /assets/images/gallery/brf-5.jpg

summer25:
  - image_path: /assets/images/gallery/summer2025.png
    excerpt: "Onboarding and Orientation of Ashoka Interns: Summer ‘25"

mmfood25:
  - image_path: /assets/images/events/Multimdal Food Computing Workshop 2025/MMFood_poster.png
  - image_path: /assets/images/events/Multimdal Food Computing Workshop 2025/MMFood_1.jpeg
  - image_path: /assets/images/events/Multimdal Food Computing Workshop 2025/MMFood_2.jpeg
  - image_path: /assets/images/events/Multimdal Food Computing Workshop 2025/MMFood_3.jpeg
  - image_path: /assets/images/events/Multimdal Food Computing Workshop 2025/MMFood_4.jpeg
  - image_path: /assets/images/events/Multimdal Food Computing Workshop 2025/MMFood_5.jpeg
  - image_path: /assets/images/events/Multimdal Food Computing Workshop 2025/MMFood_6.jpeg
  - image_path: /assets/images/events/Multimdal Food Computing Workshop 2025/MMFood_7.jpeg
  - image_path: /assets/images/events/Multimdal Food Computing Workshop 2025/MMFood_8.jpeg
  - image_path: /assets/images/events/Multimdal Food Computing Workshop 2025/MMFood_9.jpeg
  - image_path: /assets/images/events/Multimdal Food Computing Workshop 2025/MMFood_10.jpeg
  - image_path: /assets/images/events/Multimdal Food Computing Workshop 2025/MMFood_11.jpeg
    excerpt: "1st International Workshop on Multi-modal Food Computing (MMFood'25) in conjunction with the 33rd ACM International Conference on Multimedia (ACMMM25), Dublin (IE) [Oct. 2025]"

ashoka_expo25:
  - image_path: /assets/images/gallery/ashoka_expo25-1.jpg
  - image_path: /assets/images/gallery/ashoka_expo25-2.jpg
    excerpt: "Centre Expo, Ashoka University [Nov., 2025]"

ramesh_ashoka25:
  - image_path: /assets/images/gallery/ramesh25-1.jpg
  - image_path: /assets/images/gallery/ramesh25-2.jpg
    excerpt: "Prof. Ramesh Jain discussing his vision on ‘Personal Care Utility (PCU) for India’ with the Computer Science students and Phd scholars, Ashoka University [Nov. 2024]"

infuse25:
  - image_path: /assets/images/events/INFUSE Innovation Summit 2025/INFUSE_1.JPG
  - image_path: /assets/images/events/INFUSE Innovation Summit 2025/INFUSE_2.JPG
  - image_path: /assets/images/events/INFUSE Innovation Summit 2025/INFUSE_3.JPG
  - image_path: /assets/images/events/INFUSE Innovation Summit 2025/INFUSE_4.JPG
    excerpt: "INFUSE Innovation Summit, ICMR-NIN, Hyderabad (IN) [Dec. 2025]"

faf26:
  - image_path: /assets/images/events/food_alignment_forum-26/faf_1.jpeg
  - image_path: /assets/images/events/food_alignment_forum-26/faf_2.jpg
  - image_path: /assets/images/events/food_alignment_forum-26/faf_3.jpg
  - image_path: /assets/images/events/food_alignment_forum-26/faf_4.jpg
  - image_path: /assets/images/events/food_alignment_forum-26/faf_5.jpg
  - image_path: /assets/images/events/food_alignment_forum-26/faf_6.jpg
  - image_path: /assets/images/events/food_alignment_forum-26/faf_7.jpg
  - image_path: /assets/images/events/food_alignment_forum-26/faf_8.jpg
  - image_path: /assets/images/events/food_alignment_forum-26/faf_9.jpg
    excerpt: "Food Alignment Forum, Ashoka University (IN) [Feb. 2026]"

---

{% assign gallery_sets = "faf26,infuse25,ramesh_ashoka25,ashoka_expo25,mmfood25,summer25,brf25,icpr_zoom2024,icpr2024,ashoka_expo24,bdbio24" | split: "," %}

<div class="gallery-page">

{% for set_name in gallery_sets %}
{% assign gallery = page[set_name] %}

{% if gallery %}

{% assign gallery_title = "" %}
{% for item in gallery %}
{% if item.excerpt %}
{% assign gallery_title = item.excerpt %}
{% break %}
{% endif %}
{% endfor %}

{% if gallery_title != "" %}
<div class="gallery-caption">
  {{ gallery_title }}
</div>
{% endif %}

<div class="gallery-grid
  {% if gallery.size == 1 %}single-image-grid{% endif %}
  {% if gallery.size == 2 %}double-image-grid{% endif %}">

{% for item in gallery %}

<a href="{{ item.image_path }}"
   class="gallery-item"
   onclick="openLightbox('{{ item.image_path }}'); return false;">

  <img src="{{ item.image_path }}"
       alt="{{ gallery_title | strip_html | escape }}"
       loading="lazy">

</a>

{% endfor %}

</div>

<hr>

{% endif %}
{% endfor %}

</div>

<div id="lightbox" class="lightbox" onclick="closeLightbox()">
  <img id="lightbox-img" src="" alt="Expanded gallery image">
</div>

<style>

.gallery-page {
  margin-top: 20px;
}

.gallery-caption {
  text-align: center;
  margin: 10px 0 18px 0;
  font-size: 0.9rem;
  color: #b70100;
  font-weight: 400;
  line-height: 1.6;
}

.gallery-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 14px;
  margin-bottom: 24px;
  justify-items: center;
}

.gallery-item {
  position: relative;
  overflow: hidden;
  border-radius: 10px;
  background: #f3f3f3;
  width: 100%;
  max-width: 320px;
}

.gallery-item img {
  width: 100%;
  height: 100%;
  max-height: 260px;
  object-fit: contain;
  background: #f3f3f3;  
  display: block;
  cursor: zoom-in;
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}

.gallery-item img:hover {
  transform: scale(1.015);
  box-shadow: 0 10px 22px rgba(0,0,0,0.12);
}

@media (max-width: 900px) {
  .gallery-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }
}

@media (max-width: 640px) {
  .gallery-grid {
    grid-template-columns: 1fr;
  }
}

.single-image-grid {
  display: flex !important;
  justify-content: center;
}

.single-image-grid .gallery-item {
  max-width: 420px;
}

.double-image-grid {
  grid-template-columns: repeat(2, minmax(0, 420px));
  justify-content: center;
}

.single-image-grid {
  display: flex !important;
  justify-content: center;
}

.single-image-grid .gallery-item {
  max-width: 420px;
}

.lightbox {
  display: none;
  position: fixed;
  inset: 0;
  z-index: 9999;
  background: rgba(0,0,0,0.92);
  justify-content: center;
  align-items: center;
  padding: 30px;
}

.lightbox.active {
  display: flex;
}

.lightbox img {
  max-width: 95%;
  max-height: 95%;
  border-radius: 10px;
}

</style>

<script>

function openLightbox(src) {
  const lightbox = document.getElementById('lightbox');
  const img = document.getElementById('lightbox-img');

  img.src = src;
  lightbox.classList.add('active');

  document.body.style.overflow = 'hidden';
}

function closeLightbox() {
  document.getElementById('lightbox').classList.remove('active');
  document.body.style.overflow = '';
}

document.addEventListener('keydown', function(event) {
  if (event.key === 'Escape') {
    closeLightbox();
  }
});

</script>