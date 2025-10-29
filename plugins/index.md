---
layout: default
title: Plugins
permalink: /plugins/
---

<h1>Plugins</h1>
<div> plugins here</div>

<!-- 1) Grab all items from the `plugins` collection -->
{%- assign items = site.plugins -%}

<!-- 2) (Optional) Sort them. Here by 'weight' front matter, then by date desc -->
{%- assign items = items | sort: "weight" -%}
{%- assign items = items | reverse -%}

<!-- 3) Render a grid of cards -->
<div class="plugin-grid">
  {%- for item in items -%}
    <a class="plugin-card" href="{{ item.url | relative_url }}">
      <div class="thumb">
        <!-- 4) Use the 'thumb' field from each plugin's front matter -->
        <img src="{{ item.thumb | default: item.image | relative_url }}" alt="{{ item.title }}">
      </div>
      <div class="meta">
        <h2>{{ item.title }}</h2>
        {%- if item.subtitle -%}
          <p class="subtitle">{{ item.subtitle }}</p>
        {%- endif -%}
        {%- if item.tags -%}
          <ul class="tags">
            {%- for t in item.tags -%}
              <li>{{ t }}</li>
            {%- endfor -%}
          </ul>
        {%- endif -%}
      </div>
    </a>
  {%- endfor -%}
</div>

<div>end of plugins</div>
