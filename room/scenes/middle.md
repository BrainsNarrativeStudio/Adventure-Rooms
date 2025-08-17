---
id: middle
title: The Challenge
options:
  - text: "Fight bravely"
    next: end
    set:
      stats:
        experience: +5
      has:
        key: true
  - text: "Use magic"
    next: end
    if: 'has.magic'
    set:
      stats:
        experience: +8
      has:
        key: true
  - text: "Sneak around"
    next: end
    if: 'trait "Class" "=" "rogue"'
    set:
      stats:
        experience: +10
      has:
        key: true
  - text: "Try to negotiate"
    next: end
    set:
      stats:
        experience: +3
      has:
        key: false
---

{{text "name"}}, you now face your first challenge.

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
