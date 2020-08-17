---
layout: page
title: Projects
---
<div class=" project-list list-group">
{% for post in site.posts %}
    <a class="list-group-item list-group-item-action" href="{{ post.url }}">
        <div class="d-flex w-100 justify-content-between">
            <h5 class="project-link mb-1">
            {{ post.title }}
            </h5>
            <small class="project-link-date">
            {{ post.date | date_to_string: "ordinal", "US" }}
            </small>
        </div>
    </a>
{% endfor %}
</div>

