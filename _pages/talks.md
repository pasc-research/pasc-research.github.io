---
title: "Talks"
permalink: "/talks.html"
---


<div class="container">
    <div class="row justify-content-center">
        <div class="col-md-8">
        <h1 class="font-weight-bold title h6 text-uppercase mb-4">Talks</h1>
            
        {% for post in site.posts %} 
        {% if post.type == "video" %} 
        
        
        {% if post.title != null %}
          {% if group == null or group == post.group %}
         
            {% include main-loop-card.html %}
          {% endif %}
        {% endif %}
        {% endfor %}
        {% assign pages_list = nil %}
        {% assign group = nil %}

        <!-- {% endfor %} -->

        </div>
        
            <div class="col-md-4">
        {% include sidebar-featured.html %}    
    </div>
        
    </div>
</div>