---
layout: page
title: Recipes
permalink: /recipes/
---

{% assign indian_posts = site.posts | where_exp: "post", "post.categories contains 'Indian'" %}
{% if indian_posts.size > 0 %}
## 🇮🇳 Indian

{% assign chaat_posts = site.posts | where_exp: "post", "post.categories contains 'Chaat'" %}
{% if chaat_posts.size > 0 %}
### Chaat
{% for post in chaat_posts %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
{% endif %}

{% assign curries_posts = site.posts | where_exp: "post", "post.categories contains 'Curries'" %}
{% if curries_posts.size > 0 %}
### Curries
{% for post in curries_posts %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
{% endif %}

{% assign rice_posts = site.posts | where_exp: "post", "post.categories contains 'Rice & Breads'" %}
{% if rice_posts.size > 0 %}
### Rice & Breads
{% for post in rice_posts %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
{% endif %}

{% assign snacks_posts = site.posts | where_exp: "post", "post.categories contains 'Snacks & Sides'" %}
{% if snacks_posts.size > 0 %}
### Snacks & Sides
{% for post in snacks_posts %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
{% endif %}

{% assign sweets_posts = site.posts | where_exp: "post", "post.categories contains 'Sweets & Desserts'" %}
{% if sweets_posts.size > 0 %}
### Sweets & Desserts
{% for post in sweets_posts %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
{% endif %}

{% endif %}

{% assign italian_posts = site.posts | where_exp: "post", "post.categories contains 'Italian'" %}
{% if italian_posts.size > 0 %}
## 🍝 Italian
{% for post in italian_posts %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
{% endif %}

{% assign thai_posts = site.posts | where_exp: "post", "post.categories contains 'Thai'" %}
{% if thai_posts.size > 0 %}
## 🍜 Thai
{% for post in thai_posts %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
{% endif %}

{% assign backpacking_posts = site.posts | where_exp: "post", "post.categories contains 'Backpacking'" %}
{% if backpacking_posts.size > 0 %}
## 🏕️ Backpacking Recipes
{% for post in backpacking_posts %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
{% endif %}

{% assign reviews_posts = site.posts | where_exp: "post", "post.categories contains 'Restaurant Reviews'" %}
{% if reviews_posts.size > 0 %}
## 🍽️ Restaurant Reviews
{% for post in reviews_posts %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
{% endif %}

{% assign travel_posts = site.posts | where_exp: "post", "post.categories contains 'Travel Food'" %}
{% if travel_posts.size > 0 %}
## ✈️ Travel Food
{% for post in travel_posts %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
{% endif %}