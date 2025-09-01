---
id: start
title: The Pillow Fort!
options:
  - text: "Says it's Finn and I want to build"
    next: builder_path
    set:
      traits:
        Role:
          builder: "+1"
      stats:
        experience: "+1"
      text:
        characterName: "Finn"
  - text: "Tell them your name is Jake, I need to explore"
    next: explorer_path
    set:
      traits:
        Role:
          explorer: "+1"
      stats:
        experience: "+1"
        wisdom: "+1"
      text:
        characterName: "Jake"
  - text: "Say it's Marcy, and you want to learn"
    next: scholar_path
    set:
      traits:
        Role:
          scholar: "+1"
      stats:
        experience: "+1"
        wisdom: "+1"
      text:
        characterName: "Marcy"
---

You open your eyes, you find yourself in a vast, soft landscape made entirely of pillows. The air is filled with the gentle scent of fabric softener, and the ground beneath your feet is as comfortable as a cloud.

The pillow world stretches as far as the eye can see. Towering pillow mountains rise in the distance, and soft valleys wind between them. You can see pillow creatures moving about, going about their daily lives.

A friendly pillow person approaches you with a warm smile. "Welcome, traveler! I don't believe we've met. What should we call you?"

What will you do in this strange, comfortable world?