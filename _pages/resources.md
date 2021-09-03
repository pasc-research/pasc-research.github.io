---
title: "Resources"
layout: default
permalink: "/resources.html"
---

<div class="container">
<h4 class="font-weight-bold spanborder"><span>{{page.title}}</span></h4>
    <div class="row gap-y listrecent listrecent listauthor">
    {% for resource in site.resources %}
        <div class="col-lg-6 mb-4">
            <div class="p-4 border rounded">
            <div class="row">
            <div class="col-md-3 mb-4 mb-md-0"><img alt="{{ resource[1].name }}" src="{{site.baseurl}}/{{ resource[1].avatar }}" class="rounded-circle" height="80" width="80"></div>
            <div class="col-md-9">
            <a href="{{site.baseurl}}/resource-{{ resource[1].name | slugify }}">
            <h4 class="text-dark mb-0"> {{ resource[1].name }} </h4>
            <!-- <small class="d-inline-block mt-1 mb-3 font-weight-normal">(View Posts)</small> -->
            <div class="excerpt">{{ resource[1].bio }}</div>
            </a>
            <div class="icon-block mt-3 d-flex justify-content-between">  
            <div>
            <!-- <a target="_blank" href="{{ resource[1].twitter }}"><i class="fab fa-twitter text-muted" aria-hidden="true"></i></a>  &nbsp; -->
            <a target="_blank" href="{{ resource[1].site }}"><i class="fa fa-globe text-muted" aria-hidden="true"></i></a> &nbsp;
            </div>
            </div>
            </div>
            </div>
            </div>
        </div>
    {% endfor %}
    </div>
</div>