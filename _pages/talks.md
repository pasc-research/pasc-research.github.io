---
title: "Talks"
permalink: "/talks.html"


  
feature_row:
  - image_path: https://img.youtube.com/vi/vy-JUaqk1Y8/0.jpg
    alt: "placeholder image 1"
    title: "Placeholder 1"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
  - image_path: https://img.youtube.com/vi/vy-JUaqk1Y8/0.jpg
    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "placeholder image 2"
    title: "Placeholder 2"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
  
feature_row2:
  - image_path: https://img.youtube.com/vi/vy-JUaqk1Y8/0.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Left Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Left aligned with `type="left"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row3:
  - image_path: https://img.youtube.com/vi/vy-JUaqk1Y8/0.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Right Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Right aligned with `type="right"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row4:
  - image_path: https://img.youtube.com/vi/vy-JUaqk1Y8/0.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Center Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"

---




{% include feature_row.html %}

{% include feature_row.html id="feature_row2" type="left" %}

{% include feature_row.html id="feature_row3" type="right" %}

{% include feature_row.html id="feature_row4" type="center" %}