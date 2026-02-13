---
title: "Projects"
layout: collection
permalink: /projects/
collection: projects
entries_layout: grid
classes: wide
---

<div>
  {%- assign items = site.projects -%}
  {%- if items and items.size > 0 -%}
    {%- assign items = items | sort: "weight" -%}
    <div class="projects-grid">
      {%- for item in items -%}
        <a class="projects-card" href="{{ item.url | relative_url }}">
          <div class="thumb">
            <img src="{{ item.thumb | default: item.image | relative_url }}" alt="{{ item.title }}">
          </div>
          <div class="meta">
            <h2>{{ item.title }}</h2>
            {%- if item.subtitle -%}<p class="subtitle">{{ item.subtitle }}</p>{%- endif -%}
            {%- if item.tags -%}
              <ul class="tags">
                {%- for t in item.tags -%}<li>{{ t }}</li>{%- endfor -%}
              </ul>
            {%- endif -%}
          </div>
        </a>
      {%- endfor -%}
    </div>
  {%- else -%}
    <p>No items yet. Add a file to <code>/_projects/</code> with front matter to see it here.</p>
  {%- endif -%}
</div>