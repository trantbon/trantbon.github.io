---
title: Engineering Chronicles - Disc Launcher Debut
layout: post
post-image: "/assets/images/blog/disc_launcher.jpg"
description: My first CrunchLabs box.
tags:
- engineering
- robotics
- DIY
- Disc Launcher
---

<p id="play-music" style="cursor: pointer; color: blue; text-decoration: underline;">
  Click here to start the music 🎵
</p>

<audio id="bg-music" loop>
  <source src="https://cdn.voicemod.net/sounds/2023/09/9d163cb1-4d2d-4112-9845-08c762f6c313.mp3" type="audio/mpeg">
</audio>

<script>
  document.addEventListener("DOMContentLoaded", function () {
    document.getElementById("play-music").addEventListener("click", function () {
      const audio = document.getElementById("bg-music");
      audio.play().catch(function (error) {
        console.error("Playback failed:", error);
      });
    });
  });
</script>

This is the start of a series of my life to got to my dream job, an engineer...
