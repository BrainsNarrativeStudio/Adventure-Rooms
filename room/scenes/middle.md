---
id: middle
title: The Challenge2
set:
options:
  - text: "Fight bravely"
    next: complete
    set:
      stats:
        experience: "+5"
      has:
        key: true
  - text: "Use magic"
    next: complete
    set:
      stats:
        experience: "+8"
      has:
        key: true
  - text: "Sneak around"
    next: complete
    set:
      stats:
        experience: "+10"
      has:
        key: true
  - text: "Try to negotiate"
    next: complete
    set:
      stats:
        experience: "+3"
      has:
        key: false
---

{{text "name"}}, you now face your first challenge!

{{#trait "Class" "=" "warrior"}}
Your warrior's spirit burns bright. You charge forward with courage.
{{/trait}}

{{#trait "Class" "=" "mage"}}
Your magical knowledge guides you. You cast a protective spell.
{{/trait}}

{{#trait "Class" "=" "rogue"}}
Your rogue's instincts serve you well. You move with silent grace.
{{/trait}}

{{#has "sword"}}
Your sword gleams in the light.
{{/has}}

{{#has "magic"}}
Magic crackles around you.
{{/has}}

The challenge awaits your response.