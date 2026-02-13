---
layout: splash
classes: wide
title: "Spectral Processor"
author_profile: false
thumb: /assets/plugins/specGrain.png
---


<div class="plugin-content-page">
    <h1>Spectral Processor</h1>
    <div class="flex-container">
        <img src="{{ "/assets/plugins/specGrain.png" | relative_url }}"
         alt="Image of Dynamic Convolver Plugin">
    </div>
    <div class="plugin-links">
    <a href="https://github.com/Bohr33/SpecGrain_Plugin" class="btn btn-primary" target="_blank">
        <i class="fab fa-github"></i> View on GitHub
    </a>
    </div>
    <h2 class="plugin-content-page">About</h2>
    <p>The Spectral Processor began as a project for my master’s program, originally focused on implementing a phase-vocoder-based pitch-shifting system. The task proved challenging, but once the pitch shifter was working reliably, I became interested in exploring the wider creative possibilities of the phase vocoder. Using Victor Lazzarini’s Spectral Processing book as a guide for the core design, I implemented several additional algorithms featured there—including spectral blur and spectral delay.</p>
    <p>Beyond these established techniques, I introduced a new effect I call Spectral Stretch. Similar to spectral blur, this effect holds phase-vocoder frames in a buffer and processes them over time, but it adds control over the density and playback rate of the buffered frames, enabling a wider range of time-smearing and granular-like transformations.</p>
    <p>I also added an experimental feature called Freq Delay, which modifies the behavior of the spectral delay effect. Traditional implementations delay only the amplitude data, but Freq Delay optionally delays both amplitude and frequency information. In practice, this produces a unique, more pronounced spectral displacement that can be just as musically useful as amplitude only delay.</p>
</div>
