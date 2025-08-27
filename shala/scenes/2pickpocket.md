---
id: 2pickpocket
title: You feel something move in your right coat pocket
options:
  - text: "You make light of it"
    next: 3promise
    set:
      traits:
        factions:
            rebels: +1
            nihilists: +1
            exploiters: +1
  - text: "You sermon them"
    next: 3promise
    set:
      traits:
        factions:
            faithfuls: +1
  - text: "You report them"
    next: 3promise
    set:
      traits:
        factions:
            authority: +1
---

{{#trait "faction" "=" "rebels"}}
You stroll amongst the colourful stalls of the bustling street market. Fruits and vegetables galore, some that you never saw before. Suddenly, you feel a tug on your coat pocket.
{{/trait}}

{{#trait "faction" "=" "faithfuls"}}
You carefully enter the temple, where a soft melody arises from an unknown source. The monks welcome you with warm smiles, but as you move to ask them about Shangri-La, you feel a beggar tug on your coat pocket.
{{/trait}}

{{#trait "faction" "=" "authority"}}
The armory is located close to the Palace's main entrance. You see fully armed guards walking around the perimeter. As you wait for an audience with the Chief of the Guard, you observe a teenager being taken away to jail. In a split second, taking advantage of his jailors' lack of attention, the teen lunges to grab your coat pocket.
{{/trait}}

What do you do?
