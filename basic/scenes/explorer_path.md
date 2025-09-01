---
id: explorer_path
title: The Explorer's Path!
options:
  - text: "Map the entire pillow world"
    next: pillow_life
    set:
      traits:
        Role:
          explorer: "+2"
      stats:
        experience: "+2"
        wisdom: "+1"
      has:
        map: true
  - text: "Search for a way back home"
    next: resistance_path
    set:
      traits:
        Faction:
          resistance: "+2"
        Role:
          explorer: "+1"
      stats:
        experience: "+2"
        wisdom: "+1"
      has:
        map: true
  - text: "Discover the pillow world's secrets"
    next: scholar_path
    set:
      traits:
        Role:
          explorer: "+1"
          scholar: "+1"
      stats:
        experience: "+2"
        wisdom: "+2"
---

You choose to explore, and the pillow world reveals its vastness to you. There are hidden valleys, secret passages, and mysterious landmarks that the pillow people have never ventured to.

{{#trait "Role" "=" "explorer"}}
**Your explorer instincts are perfectly suited to this world. You notice details others miss and find paths that seem invisible to them.**
{{/trait}}

As you explore, you begin to understand the true scope of this place. It's not just a collection of pillows - it's a complete world with its own geography, climate, and hidden wonders.

{{#stat "wisdom" ">" 1}}
**Your growing wisdom helps you understand the patterns and logic of this strange world's layout.**
{{/stat}}

What will you discover first?