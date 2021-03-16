---
layout: post
title:  "First Post"
date:   2021-03-16 17:04:49 +0000
categories: General
---

Suppose I should write something in here. Thought it might be a good place to keep track of my
various hobbies and interests. 

Hopefully I'll be able to keep this up for a while, particularly for keeping track of my motorbike
stuff. Since it's something I currently have no experience in it might be nice to come back to
this later and see how my skills have developed. 

Let's wait and see. 


<div class="post-categories">
  Tags: &nbsp; 
  {% if post %}
    {% assign categories = post.categories %}
  {% else %}
    {% assign categories = page.categories %}
  {% endif %}
  {% for category in categories %}
  <a href="{{site.baseurl}}/categories/#{{category|slugize}}">{{category}}</a>
  {% unless forloop.last %}&nbsp;{% endunless %}
  {% endfor %}
</div>