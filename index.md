---
title: Home
photos:
  - image: /uploads/23.jpg
  - image: /uploads/22.jpg
  - image: /uploads/0.png
  - image: /uploads/1.jpg
  - image: /uploads/2.jpg
  - image: /uploads/3.jpg
  - image: /uploads/4.jpg
  - image: /uploads/5.jpg
  - image: /uploads/6.jpg
  - image: /uploads/7.jpg
  - image: /uploads/8.jpg
  - image: /uploads/9.jpg
  - image: /uploads/10.jpg
  - image: /uploads/11.jpg
  - image: /uploads/12.jpg
  - image: /uploads/13.jpg
  - image: /uploads/14.jpg
  - image: /uploads/15.jpg
  - image: /uploads/16.jpg
  - image: /uploads/17.jpg
  - image: /uploads/18.jpg
  - image: /uploads/19.jpg
  - image: /uploads/20.jpg
  - image: /uploads/21.jpg
---

<ul class="gallery">
  {% for photo in page.photos %}
  <li style="background-image: url('{{ site.baseurl }}{{ photo.image | resize: " 800x800>
    " }}')"><a
      title="{{ photo.caption | '' }}"
      href="{{ site.baseurl }}{{ photo.image }}"
      data-id="#{{ photo.image | slugify }}"
      data-caption="{{ photo.caption | '' }}"
    ></a>
  </li>
  {% endfor %}
  <li class="spacer"></li>
  <li class="spacer"></li>
  <li class="spacer"></li>
  <li class="spacer"></li>
  <li class="spacer"></li>
  <li class="spacer"></li>
  <li class="spacer"></li>
  <li class="spacer"></li>
  <li class="spacer"></li>
  <li class="spacer"></li>
  <li class="spacer"></li>
  <li class="spacer"></li>
</ul>

<div class="overlay">
  <a href="#" class="close">&#10005;</a>
  <a class="prev">&lsaquo;</a>
  <a class="next">&rsaquo;</a>
  <p class="caption"></p>
  <img />
</div>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
<script>
  var script = document.createElement('script');
  script.src = '{{ site.baseurl }}/js/lightbox.js';
  document.body.appendChild(script);
</script>
