---
title: "Resources"
permalink: "/resources.html"
---


<div class="container">
    <div class="row justify-content-center">
        <div class="col-md-8">
            
        {% for post in site.posts %} 
        {% if post.tags contains "video" %}
        
         
            {% include main-loop-card.html %}
          
        {% endif %}

        {% endfor %}

        </div>
        
            <div class="col-md-4">
        {% include sidebar-featured.html %}    
    </div>
        
    </div>
</div>