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

This is the start of a series of my life to got to my dream job, an engineer. I will be posting after I finish one blog about my day to day life and what I do to become an engineer. In here is information about what I have learned about the robot that I had to build, the disc launcher.
Today, I received my first ever CrunchLabs box made Mark Rober. Each month, Mark sends out a new box with parts that you use to build with a video explaining the physics and how to build the robot. Since I just started, I got the easiest build challenge which was a disc launcher. There was many parts used to build it, but the most important part was the flywheel. It is a hollow, heavy wheel that spins and stores up kinetic energy but spinning at very high rates.
