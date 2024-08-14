# Demiplane 2 Roll20
A tool that enables rolls from Demiplane character sheets to be rolled in Roll20.

Note that this tool does not use the Roll20 api and so should not require you to be a Pro member to make use of it.

This tool is also compatible with the new Discord Activity for Roll20.

## Overview
This is a ```UserScript```, meaning it needs to be used with a browser extension like [TamperMonkey](https://chromewebstore.google.com/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo) or [ViolentMonkey](https://chromewebstore.google.com/detail/violentmonkey/jinjaccalgkegednnccohejagnlnfdag) etc.

Once you have one of those extensions, you can enable it by clicking the install button on this page:
https://greasyfork.org/en/scripts/503467-demiplane-2-roll20

When enabled, it creates a communication layer between Demiplane and Roll20, allowing rolls made in your Demiplane character sheet to automatically appear in Roll20 (with the same roll result that shows in Demiplane).

## Getting Started

Once you have added the userscript to your extension of choice and enabled it, you have everything you need.

Each time you open Roll20, you should see an extra bit of ui under the chat box labelled 'Enable rolls from Demiplane'.
This checkbox defaults to off whenever you open a new Roll20 session to prevent you from making rolls accidentally.

If you check the checkbox, any rolls made from any Demiplane character sheet open in any of your browser tabs will be "funneled" to Roll20 and appear in the Roll20 chat. Keep in mind you must have both Roll20 and Demiplane open in the same browser for this to work.

## Game Specific Features

Lots of games have particular features tied to certain roll results/specialty dice, etc. I've done my best to handle all of these in this tool and any "Special" results, should automatically appear in a section of the roll labelled "Modifiers". I've done this for all games currently available in Demiplane but keep in mind that as new games get added these mechanics will probably not work until I spend a little time adding handling for them.
Below is a list of these features by game (please let me know if I have missed any big ones):

Cosmere RPG: Opportunity, Complication

Marvel RPG: Fantastic, Ultimate Fantastic

Avatar Legends: Miss/Weak/Strong Hit

Daggerheart: Hope, Fear, Critical Success

Candela Obscura: Critical Success

Starfinder: Natural 20s

Pathfinder: Natural 20s

Alien RPG: Panic

Vampire the Masquerade: Messy Critical, Bestial Failure, Standard Critical

## Caveats/Known Issues:

-I've tested with all currently available character sheets in Demiplane and I think everything should be working but if new sheets are added it may take me a little bit to add them to implementation, there are small code changes I need to make if new sheet types get added.

-If you collapse your roll results, the tool can only show what is in the collapsed view in roll20. This means the subheader and other things that are hidden in collapsed mode will not appear in Roll20. The tool should work as normal otherwise, and if you want the additional information, just toggle the dice view to be uncollapsed.
