---
id: 3promise
title: Make A Promise

options:
  - text: You Accept
    next: 4coverup

    set:
        stats:
            explore: +1

    if: 'trait "factions" "=" "rebels"'
    set:
      traits:
        factions:
            rebels: +1
            authority: -1

    if: 'trait "factions" "=" "faithfuls"'
    set:
      traits:
        factions:
            faithfuls: +1

    if: 'trait "factions" "=" "authority"'
    set:
      traits:
        factions:
            rebels: -1
            authority: +1

  - text: You Refuse
    next: 4coverup

    set:
        stats:
            leave: +1

    if: 'trait "factions" "=" "rebels"'
    set:
      traits:
        factions:
            rebels: -1
            authority: +1

    if: 'trait "factions" "=" "faithfuls"'
    set:
      traits:
        factions:
            faithfuls: -1

    if: 'trait "factions" "=" "authority"'
    set:
      traits:
        factions:
            rebels: +1
            authority: -1

---

You seem trustworthy. 

{{#trait "faction" "=" "rebels"}}
A vendor from the market approaches you. Their eyes are intently set on you. 
{{/trait}}

{{#trait "faction" "=" "faithfuls"}}
A monk takes you aside. They whisper to you: "You finally made it."
{{/trait}}

{{#trait "faction" "=" "authority"}}
After the commotion dies down, one guard turns to you.
{{/trait}}

They seem frazzled and urge you to make them a promise.