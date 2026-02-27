---
layout: splash
classes: wide
title: "Dynamic Convolver"
author_profile: false
thumb: /assets/plugins/dynamic-convolver.png
excerpt: "A convolution reverb plugin that allows dynamic selection of the convolution region of a user uploaded impulse response file. Also features an array of additional pre- and post-proceessing."
---


  

<div class="plugin-content-page">
<h1>Dynamic Convolver</h1>
      <img src="{{ page.thumb }}"
        alt="Image of Dynamic Convolver Plugin">
  <div>  
    <div class="title-text">
      <p> The Dynamic Convolver is a convolution plugin that implements the standard convolution algorithm with the additional ability to edit the convolution file in real-time for experimental sound design. The goal for this plugin was to make it easy to experiment with different Impulse Response files during real-time convolution processing. This plugin makes this easy by providing an editable region of uploaded file that can be altered in real-time. </p>
      <p>The main control window gives users control over the start position, region length, and playback speed (which also doubles as a tuning parameter). Additional processing controls in the pre and post sections allow for precise shaping of the input and output signal, opening up a wide range of sonic experimentation.</p>
    </div>
  </div>
</div>

<h2>Audio Demo</h2>
The examples below showcase various convolution processing results using different impulse response files. Each file is the convolution processing result between the raw file, and the description of the file above. 
<div class="audio-demo">
  <div class="unprocessed">
      <p>Raw Piano</p>
    <audio controls style="width:100%;">
      <source src="/assets/audio/DynamicConvolver/Raw Piano-MP3.mp3" type="audio/mpeg">
    </audio>
  </div>
  <div class="audio-player">
      <p>Cathedral</p>
    <audio controls style="width:100%;">
      <source src="/assets/audio/DynamicConvolver/Piano_Cathedral-MP3.mp3" type="audio/mpeg">
    </audio>
  </div>
  <div class="audio-player">
      <p>Reversed Cathedral</p>
    <audio controls style="width:100%;">
      <source src="/assets/audio/DynamicConvolver/Reversed_Piano-MP3.mp3" type="audio/mpeg">
    </audio>
  </div>
  <div class="audio-end">
     <p>Bass Drum</p>
    <audio controls style="width:100%;">
      <source src="/assets/audio/DynamicConvolver/Piano_BassDrum-MP3.mp3" type="audio/mpeg">
    </audio>
  </div>
</div>


<div class="audio-demo">
  <div class="unprocessed">    
      <p>Raw Drums</p>
    <audio controls style="width:100%;">
      <source src="/assets/audio/DynamicConvolver/Drums_Raw-MP3.mp3" type="audio/mpeg">
    </audio>
  </div>
    <div class="audio-player">
      <p>Reverse Hall</p>
    <audio controls style="width:100%;">
      <source src="/assets/audio/DynamicConvolver/Drums_HallRev-MP3.mp3" type="audio/mpeg">
    </audio>
  </div>
  <div class="audio-player">
      <p>Piano Chord</p>
    <audio controls style="width:100%;">
      <source src="/assets/audio/DynamicConvolver/Drums_Dorian-MP3.mp3" type="audio/mpeg">
    </audio>
  </div>
  <div class="audio-player">
      <p>Synth Growl</p>
    <audio controls style="width:100%;">
      <source src="/assets/audio/DynamicConvolver/Drums_BassGrowl-MP3.mp3" type="audio/mpeg">
    </audio>
  </div>
  <div class="audio-end">
      <p>Synth FX</p>
    <audio controls style="width:100%;">
      <source src="/assets/audio/DynamicConvolver/Drums_Hops-MP3.mp3" type="audio/mpeg">
    </audio>
  </div>
</div>


## Download and Links

<div class="link-container">
  <div class="plugin-links">
      <a href="https://github.com/Bohr33/CabbagePlugins" class="btn btn-primary" target="_blank">
          <i class="fab fa-github"></i> View on GitHub
      </a>
  </div>
  <div class="plugin-links">
    <a href="https://www.youtube.com/watch?v=oetY_9h6XeM" class="btn btn-primary" target="_blank">
        <i class="fab fa-youtube"></i> Watch on YouTube
    </a>
  </div>
</div>


<h2>Technical Details</h2>
- **Format**: Component (`.component`)
- **Built With**: Csound & Cabbage
- **OS**: macOS

Note: This plugin is not actively maintained. It is provided as-is for demonstration purposes. If you encounter issues, feel free to reach out but support may be limited.


