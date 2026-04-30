---
layout: splash
classes: wide
title: "Plugins"
author_profile: false
header:
  overlay_image: /assets/images/panular.png
  overlay_filter: 0.5
title: Plugins
permalink: /plugins/
---

<div>
  <p>As an audio programmer who is interested in the creative applications of DSP, one of my favorite ways of experimenting with and learning about new DSP effects is by creating a plugin with the effect. This not only gives me experience working with the DSP on a hands on level, but also creates a meaningful and useful tool once done. Because I've made of many of these devices for school and other projects, I've decided to host them all here to both showcase my work, and allow others to download and expirement with them as well</p>
  
  <p>All of the plugin pages contain links to my github where the source code can be downloaded. Some of these plugins were made with tools like Csound, Max/MSP, and RNBO, while others are in C++ with JUCE or other libraries. Each page will highlight the language used, as well as outline any intersting methods if relevant</p>

  {%- assign items = site.vsts -%}
  {%- if items and items.size > 0 -%}
    {%- assign items = items | sort: "weight" -%}
    <div class="plugin-grid">
        {%- for item in items -%}
      <div class="plugin-card">
        <div class="meta">
          <h2>{{ item.title }}</h2>
          {%- if item.subtitle -%}<p class="subtitle">{{ item.subtitle }}</p>{%- endif -%}
        </div>
          <a class="plugin-card-body" href="{{ item.url | relative_url }}">
            <div class="plugin-thumbnail">
              <img src="{{ item.thumb | default: item.image | relative_url }}" alt="{{ item.title }}">
            </div>
            <div class="thumb-text">
              <p>{{item.excerpt}}</p>
            </div>
          </a>
      </div>
        {%- endfor -%}
    </div>
  {%- else -%}
    <p>No items yet. Add a file to <code>/_vsts/</code> with front matter to see it here.</p>
  {%- endif -%}
</div>
