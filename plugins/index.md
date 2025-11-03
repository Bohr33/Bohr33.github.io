---
layout: splash
classes: wide
title: "Plugins"
author_profile: false
header:
  overlay_image: /assets/images/output.png
  overlay_filter: 0.5
title: Plugins
permalink: /plugins/
---

<div>
  <h1>Plugins</h1>
  <p>As an audio programmer who is interested in the creative applications of DSP, one of my favorite ways of experimenting with and learning about new DSP effects is by creating a plugin with the effect. This not only gives me experience working with the DSP on a hands on level, but also creates a meaningful and useful tool once done. Because I've made of many of these devices for school and other projects, I've decided to host them all here to both showcase my work, and allow others to download and expirement with them as well</p>
  
  <p>All of the plugin pages contain links to my github where the source code can be downloaded. Some of these plugins were made with tools like Csound, Max/MSP, and RNBO, while others are in C++ with JUCE or other libraries. Each page will highlight the language used, as well as outline any intersting methods if relevant</p>

  {%- assign items = site.vsts -%}
  {%- if items and items.size > 0 -%}
    {%- assign items = items | sort: "weight" -%}
    <div class="plugin-grid">
      {%- for item in items -%}
        <a class="plugin-card" href="{{ item.url | relative_url }}">
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
    <p>No items yet. Add a file to <code>/_vsts/</code> with front matter to see it here.</p>
  {%- endif -%}
</div>
