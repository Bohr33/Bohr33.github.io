---
layout: splash
classes: wide
title: "PVExperiments"
author_profile: false
thumb: /assets/plugins/PVExperiments_Screenshot.png
excerpt: "An experimental spectral processing plugin that features some basic, and experimental, effects that utilize the spectral capabilities of the Phase Vocoder. Features pitch shifting, blur, stretch, and spectral delay with additional parameters."
order: 2
---


<div class="plugin-content-page">
    <h1>PVExperiments</h1>
    <div class="flex-container">
        <img src="{{ "/assets/plugins/PVExperiments_Screenshot.png" | relative_url }}"
         alt="Image of Spectral Processor Plugin">
    </div>



    <h2 class="plugin-content-page">About</h2>
    <p>PVExperiments began as a project for my master’s program, originally focused on implementing a phase-vocoder-based pitch-shifting system. The task proved challenging, but once the pitch shifter was working reliably, I became interested in exploring the wider creative possibilities of the phase vocoder. Using Victor Lazzarini’s Spectral Processing book as a guide for the core design, I implemented several additional algorithms featured there—including spectral blur and spectral delay.</p>
    <p>Beyond these established techniques, I introduced a new effect I call Spectral Stretch. Similar to spectral blur, this effect holds phase-vocoder frames in a buffer and processes them over time, but it adds control over the density and playback rate of the buffered frames, enabling a wider range of time-smearing and granular-like transformations.</p>
    <p>I also added an experimental feature called Freq Delay, which modifies the behavior of the spectral delay effect. Traditional implementations delay only the amplitude data, but Freq Delay optionally delays both amplitude and frequency information. In practice, this produces a unique, more pronounced spectral displacement that can be just as musically useful as amplitude only delay.</p>
</div>



<div class="audio-demo">
    <div class="audio-player">
        Original Audio
    <audio controls style="width:100%;">
        <source src="/assets/audio/SpecGrain/Synth_Raw-MP3.mp3" type="audio/mpeg">
    </audio>
    </div>
    <div class="audio-player">
        Pitch Shift
    <audio controls style="width:100%;">
        <source src="/assets/audio/SpecGrain/Synth_Repitch-MP3.mp3" type="audio/mpeg">
    </audio>
    </div>
    <div class="audio-player">
        Spectral Blur
    <audio controls style="width:100%;">
        <source src="/assets/audio/SpecGrain/Synth_Blur-MP3.mp3" type="audio/mpeg">
    </audio>
    </div>
    <div class="audio-player">
        Spectral Stretch
    <audio controls style="width:100%;">
        <source src="/assets/audio/SpecGrain/Synth_Stretch-MP3.mp3" type="audio/mpeg">
    </audio>
    </div>
    <div class="audio-player">
        Spectral Delay
    <audio controls style="width:100%;">
        <source src="/assets/audio/SpecGrain/Synth_SpecDelay-MP3.mp3" type="audio/mpeg">
    </audio>
    </div>
    <div class="audio-player">
        Spectral Delay with Frequency Toggle
    <audio controls style="width:100%;">
        <source src="/assets/audio/SpecGrain/Synth_FreqDelay-MP3.mp3" type="audio/mpeg">
    </audio>
    </div>
</div>

<div class="plugin-links">
    <a href="https://github.com/Bohr33/SpecGrain_Plugin" class="btn btn-primary" target="_blank">
        <i class="fab fa-github"></i> View on GitHub
    </a>
    <a href="https://youtu.be/9RQPw5KCHsc" class="btn btn-primary">
    <i class="fab fa-youtube"></i> View on Youtube>
</div>