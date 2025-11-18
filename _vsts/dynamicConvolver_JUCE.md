---
layout: splash
classes: wide
title: "Dynamic Convolver (JUCE)"
author_profile: false
thumb: /assets/plugins/dConv(JUCE).png
---


<div class="plugin-content-page">
    <h1>Dynamic Convolver</h1>
    <div class="flex-container">
        <img src="{{ "/assets/plugins/dConv(JUCE).png" | relative_url }}"
         alt="Image of Dynamic Convolver Plugin">
    </div>
    <h2 class="plugin-content-page">About</h2>
    <p>This project began as an exercise in C++ programming with JUCE, inspired by a convolution plugin I originally developed during my undergraduate studies using Csound and Cabbage, titled the <em>Dynamic Convolver</em>. That earlier version implemented standard convolution processing but allowed the user to isolate a specific region of an impulse response or audio file and manipulate the processing position in real time. This new version represents my attempt to recreate and expand that concept entirely in C++ within the JUCE framework.</p>


<h3>Development</h3>
<p>One of the most significant challenges in developing this plugin was implementing the convolution engine from scratch. While JUCE provides a built-in convolution module, it does not expose enough of its internal processing to support the level of customization I needed. As a result, I wrote my own convolution class to gain full control over the DSP flow and enable more experimental features.</p>

<h3>Features</h3>
<p>In its current state, this version of the Dynamic Convolver functions like a standard convolution processor: users can load an impulse response (or any audio file) and adjust the Dry/Wet control to blend the processed signal. The novel functionality comes from the file-positioning controls and visual display. Once a file is loaded, it appears on the GUI, and the <strong>File Position</strong> and <strong>File Length</strong> parameters define a highlighted region—representing the portion of the file used for convolution. This allows users to “focus” the convolution on any segment of the impulse response.</p>

<p>At present, adjusting the File Position parameter during real-time playback may produce choppy results due to the abrupt shift in the convolution window. Future updates aim to smooth this behavior, likely through interpolation or buffered transitions, improving performance for dynamic, real-time manipulation.</p>

    
</div>
