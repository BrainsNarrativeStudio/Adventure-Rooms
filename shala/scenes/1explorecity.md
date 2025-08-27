---
id: 1explorecity
title: Explore The City
options:
  - text: "Talk to common folks at the market"
    next: 2pickpocket
    set:
      traits:
        factions: 
            rebels: +1
  - text: "Talk to monks in the temple"
    next: 2pickpocket
    set:
      traits:
        factions: 
            faithfuls: +1
  - text: "Talk to the guards in the armory"
    next: 2pickpocket
    set:
      traits:
        factions: 
            authority: +1
---

You are fascinated by this new world you have discovered. You simply MUST find out what the heck is happening here.

{{#stats "explore" "=" 1}}
You're so excited to get going.
{{/stats}}

{{#stats "leave" "=" 1}}
You're weary of this place, it all seems to good to be true.
{{/stats}}

What do you want to do next?
