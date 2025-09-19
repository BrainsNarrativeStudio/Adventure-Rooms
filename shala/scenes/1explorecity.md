---
id: 1explorecity
title: Explore The City
set:
options:
  - text: "Talk to common folks at the market"
    next: scene_1758314839014
    set:
      traits:
        faction:
          rebels: "+1"
  - text: "Talk to monks in the temple"
    next: scene_1758314899776
    set:
      traits:
        faction:
          faithfuls: "+1"
  - text: "Talk to the guards in the armory"
    next: scene_1758314876554
    set:
      traits:
        faction:
          authority: "+1"
---

You are fascinated by this new world you have discovered. You simply MUST find out what the heck is happening here.

{{#stat "explore" "=" 1}}
You're so excited to get going.
{{/stat}}

{{#stat "leave" "=" 1}}
You're weary of this place, it all seems to good to be true.
{{/stat}}

What do you want to do next?