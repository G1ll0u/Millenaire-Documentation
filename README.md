# Millenaire-documentation
#### A WIP documentation and tweaking project about our old Millénaire 1.12.2 mod

Fixes, tweaks and documentation about Millénaire mod 1.12.2
Here will simply be some things I do for the good old Millénaire mod. My goal is to make some documentation and edit cultures to fix bugs or add features.

Mainly focused on controlled villages.

I'm not a developer, I just take advantage of how good this mod is made because every file related to culture is simple plain text 

## Introduction to how Millénaire cultures work
The principle of millénaire is that you have cultures :
**byzantines**  **indian**  **inuits**  **japanese**  **mayan**  **norman**  **seljuk**

I will focus on normans because it's the most complete culture.

Every culture has villagers, here are some :
**farmer wife boy girl**

Every villagers have goals here are some :
**makebread plantwheat harvestwheat childeatapples godrinkdider**

Their housing :
**armoury bakery quarry**

You can play with all these aspects by simply manipulating txt files.
* You can create or edit goals

### Deployment
When you install Millénaire for the first time, it deploys all its cultures data and settings in '/mods/millénaire' AND '/mods/millenaire-custom'.

#### folder '/mods/millénaire'
"The millenaire/ directory is auto-deployed by Millénaire on each new version of the mod, erasing all changes made to it.
This folder contains all the base files of every cultures, again it's all really human readable plain text, it will help when creating a culture

#### folder '/mods/millénaire-custom'
It's here that you will add things !

## Files and directory structures
Here is the directory tree of /mods/millénaire with simple explanations :

```
millenaire
├── cultures | folder that contains all cultures (I only listed normans here)
│   ├── norman
│   │   ├── buildings       | contains all generated buildings
│   │   ├── custombuildings | contains all controlled village buildings
│   │   ├── lonebuildings   | contains all lonebuildings you see sometimes
│   │   ├── namelists       | villagers namelist
│   │   ├── shops           | don't know
│   │   ├── villagers       | contains all villagers types (wife, farmer etc.)
│   │   ├── villages        | contains villages configuration files
│   │   └── walls           | contains walls related things
├── goals | contains all goals for every culture / villagers !
│   ├── genericcooking | cooking goals
│   ├── genericcrafting | crafting goals
│   ├── genericgatherblocks | etc.
│   ├── genericharvesting 
│   ├── genericmining
│   ├── genericplanting
│   ├── genericplantsapling
│   ├── genericslaughteranimal
│   ├── generictakefrombuilding | resource transport from building ?
│   ├── generictendfurnace
│   └── genericvisit | goals like "goDrinkCider
├── help | helpful documentation
├── languages
│ 
├── quests
│   ├── byzantinesbasic
│   ├── common
│   ├── indianbasic
│   ├── inuitbasic
│   ├── japanesebasic
│   ├── marvel-norman
│   ├── mysterybasic
│   ├── normanbasic
│   ├── seljukbasic
│   ├── worldquest-indian
│   ├── worldquest-mayan
│   └── worldquest-norman
└── villagerconfig 
├── blocklist.txt | Don't know
├── blocktypes.txt | Allows to whitelist blocks so they can build or spawn on it (can be useful when encountering problems with other mods)
├── Colour Sheet.png
├── config-server.txt | default server config file
├── config.txt | default client config file
├── Content creation readme.txt
├── hof.txt | hall of fame
├── itemlist.txt | list of items
├── version.txt
└── WARNING - changes here will be overwritten on update.txt

```

