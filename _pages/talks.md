---
title: "Talks"
permalink: "/talks.html"


header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  
images:
  - image: https://img.youtube.com/vi/vy-JUaqk1Y8/0.jpg
  - image: https://img.youtube.com/vi/vy-JUaqk1Y8/0.jpg
  - image: https://img.youtube.com/vi/vy-JUaqk1Y8/0.jpg

---


{% for item in page.images %}
<div class="lightbox" id="lightbox{{ forloop.index }}">
  <div class="table">
    <div class="table-cell">
      <!-- <img class="close" src="/img/close.svg" />
      <img class="next" src="/img/next.svg" />
      <img class="prev" src="/img/prev.svg" /> -->
      <div class="item" style="background: url('{{ item.image }}') center center no-repeat; background-size: cover;">
      </div>
    </div>
  </div>
</div>
{% endfor %}
