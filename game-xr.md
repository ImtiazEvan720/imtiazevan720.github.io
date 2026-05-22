---
layout: page
title: Game / XR / Graphics Projects
subtitle: Unity, Unreal, AR/VR, shaders, runtime assets, and immersive applications
permalink: /game-xr/
---

<div class="home-intro" style="text-align:center; margin-bottom: 2rem;">
  <p style="font-size: 1.1rem;">
    Selected projects involving Unity3D, Unreal Engine, AR/VR, shaders, runtime asset systems, WebGL, and interactive 3D tools.
  </p>
</div>

{% assign projects = site.posts | where_exp: "post", "post.categories contains 'game-xr'" %}

{% if projects.size > 0 %}
  <div class="row">
    {% for post in projects %}
      <div class="col-md-6" style="margin-bottom: 1.5rem;">
        <div style="border: 1px solid #ddd; border-radius: 14px; padding: 1.25rem; height: 100%; box-shadow: 0 4px 12px rgba(0,0,0,0.06);">
          <div style="font-size: 2rem; margin-bottom: 0.5rem;">🎮</div>

          <h3>
            <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
          </h3>

          {% if post.subtitle %}
            <p><strong>{{ post.subtitle }}</strong></p>
          {% endif %}

          <p>{{ post.excerpt | strip_html | truncate: 180 }}</p>

          <a href="{{ post.url | relative_url }}">Read more →</a>
        </div>
      </div>
    {% endfor %}
  </div>
{% else %}
  <p>No Game / XR projects found yet.</p>
{% endif %}
