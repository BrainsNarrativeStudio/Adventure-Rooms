---
id: 3promise
title: Make A Promise

options:
  - text: You Accept
    next: 4coverup
    if: 'trait "factions" "=" "rebels"'
    set:
      stats:
        explore: +1
      traits:
        factions:
          rebels: +1
          authority: -1

  - text: You Accept
    next: 4coverup
    if: 'trait "factions" "=" "faithfuls"'
    set:
      stats:
        explore: +1
      traits:
        factions:
          faithfuls: +1

  - text: You Accept
    next: 4coverup
    if: 'trait "factions" "=" "authority"'
    set:
      stats:
        explore: +1
      traits:
        factions:
          rebels: -1
          authority: +1

  - text: You Refuse
    next: 4coverup
    set:
      stats:
        leave: +1
      traits:
        factions:
          rebels: -1
          authority: +1
          faithfuls: -1

---

You seem trustworthy. 

{{#trait "factions" "=" "rebels"}}
A vendor from the market approaches you. Their eyes are intently set on you. 
{{/trait}}

{{#trait "factions" "=" "faithfuls"}}
A monk takes you aside. They whisper to you: "You finally made it."
{{/trait}}

{{#trait "factions" "=" "authority"}}
After the commotion dies down, one guard turns to you.
{{/trait}}

They seem frazzled and urge you to make them a promise.
