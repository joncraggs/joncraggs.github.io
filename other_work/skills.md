---
layout: page
title: Archery & Horseriding
permalink: /skills/
images:
    - image:
        path: images/Archery.jpg
        title: Archery
    - image: 
        path: images/Horseriding.jpg
        title: Horseriding
    - image: 
        path: images/HorseArchery.jpg
        title: Horse Archery
    - image: 
        path: images/BADC.jpg
        title: BADC Combat
---

Bryony Reynolds is the current champion in American Flatbow (traditional) archery for Oxfordshire, GB. 
Awards include:
- Gold medalist - County of Oxfordshire JIN Indoor competition 2022 
- Gold medalist - County of Oxfordshire Senior Outdoor Championships 2022

She is also trained in horseback archery, horse riding, and BADC rapier, dagger and unarmed combat for stage and screen.

<div class="youtube-embed">
    <iframe src="https://player.vimeo.com/video/696070099?" width="640" height="360" frameborder="0" allow="autoplay; fullscreen" allowfullscreen="" id="yui_3_17_2_1_1608744716903_103"></iframe>
</div>

<ul class="gallery">
    {%- for rawimage in page.images -%}
    {%- assign image = rawimage.image -%}
    <li>
        <img src="{{ site.url }}/{{ image.path }}" alt="{{ image.title }}" onclick="overlayImage(this)"/>
        <span>{{image.title}}</span>
    </li>
    {%- endfor -%}
</ul>
<div class="gallery-overlay">
    <div class="gallery-image-container">
        <a href="javascript:void(0);" class="close-button" onclick="closeOverlay()">
            <span></span>
            <span></span>
            <span></span>
        </a>
        <img id="gallery-image"/>
        <a href="javascript:void(0);" class="prev-button" onclick="galleryPrev()">
            <span></span>
            <span></span>
            <span></span>
        </a>
        <a href="javascript:void(0);" class="next-button" onclick="galleryNext()">
            <span></span>
            <span></span>
            <span></span>
        </a>
    </div>
</div>
