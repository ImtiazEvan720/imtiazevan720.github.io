---
layout: page
title: Projects
subtitle: "Selected software engineering, full-stack, game/XR, graphics, and systems work"
permalink: /projects/
---

<div class="home-intro" style="text-align:center; margin-bottom: 2rem;">
  <p style="font-size: 1.1rem;">
    A collection of selected projects across full-stack web development, cloud systems, Unity/Unreal XR applications, graphics tools, and HPC/system automation.
  </p>
</div>

{% assign projects = site.posts %}

{% if projects.size > 0 %}
  <div class="row">
    {% for post in projects %}

      {% if post.categories contains "game-xr" %}
        {% assign fallback_icon = "🎮" %}
      {% elsif post.categories contains "systems" %}
        {% assign fallback_icon = "⚙️" %}
      {% elsif post.categories contains "fullstack" %}
        {% assign fallback_icon = "💻" %}
      {% else %}
        {% assign fallback_icon = "📁" %}
      {% endif %}

      <div class="col-md-6" style="margin-bottom: 1.5rem;">
        <div style="border: 1px solid #ddd; border-radius: 14px; overflow: hidden; height: 100%; box-shadow: 0 4px 12px rgba(0,0,0,0.06); background: #fff;">

          {% if post.thumbnail-img %}
            <a href="{{ post.url | relative_url }}">
              <img
                src="{{ post.thumbnail-img | relative_url }}"
                alt="{{ post.title }} thumbnail"
                style="width: 100%; height: 210px; object-fit: cover; display: block;"
                onerror="this.style.display='none'; this.parentElement.nextElementSibling.style.display='flex';"
              >
            </a>

            <div style="height: 210px; display:none; align-items:center; justify-content:center; background:#f5f5f5; font-size: 3rem;">
              {{ fallback_icon }}
            </div>
          {% else %}
            <div style="height: 210px; display:flex; align-items:center; justify-content:center; background:#f5f5f5; font-size: 3rem;">
              {{ fallback_icon }}
            </div>
          {% endif %}

          <div style="padding: 1.25rem;">

            <div style="font-size: 1.8rem; margin-bottom: 0.5rem;">
              {{ fallback_icon }}
            </div>

            <h3 style="margin-top: 0;">
              <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
            </h3>

            {% if post.subtitle %}
              <p><strong>{{ post.subtitle }}</strong></p>
            {% endif %}

            <p>{{ post.excerpt | strip_html | truncate: 180 }}</p>

            {% if post.categories %}
              <p style="font-size: 0.9rem; color: #666;">
                {% for category in post.categories %}
                  <span style="display:inline-block; margin-right: 0.4rem; margin-bottom: 0.35rem; padding: 0.15rem 0.45rem; border: 1px solid #ddd; border-radius: 999px;">
                    {{ category }}
                  </span>
                {% endfor %}
              </p>
            {% endif %}

            <a href="{{ post.url | relative_url }}">Read more →</a>
          </div>

        </div>
      </div>
    {% endfor %}
  </div>
{% else %}
  <p>No projects found yet.</p>
{% endif %}
