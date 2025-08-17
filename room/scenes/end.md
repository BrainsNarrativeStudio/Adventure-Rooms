---
id: end
title: The End
---

{{text characterName}}, your journey has ended.

{{#if visited "start"}}
You began at the crossroads of destiny.
{{/if}}

{{#if visited "middle"}}
You faced the challenge with courage.
{{/if}}

{{#if has.key}}
You found the key to success.
{{/if}}

{{#if trait "Class" "=" "warrior"}}
Your warrior's path has made you strong.
{{/if}}

{{#if trait "Class" "=" "mage"}}
Your magical path has made you wise.
{{/if}}

{{#if trait "Class" "=" "rogue"}}
Your rogue's path has made you clever.
{{/if}}

The story is complete.
