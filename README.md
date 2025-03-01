# Millenaire-fixes
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
**carpenter  cattlefarmerfemale  cattlefarmermale  ciderproducer  farmer  glassblower  guard  herbalist  lumberman  miner  monk  pigherd  pigherdf  priest  shepherd  smith  weaver  wife**

Every villagers have goals here are some :
**makebread plantwheat harvestwheat childeatapples godrinkdider**

They need housing :
**armoury bakery quarry**

You can play with all these aspects by simply manipulating txt files.

## Files and directory structures
```
├── cultures
│   ├── norman
│   │   ├── buildings       | contains all generated buildings
│   │   ├── custombuildings | contains all controlled village buildings
│   │   ├── lonebuildings   | contains all lonebuildings you see sometimes
│   │   ├── namelists       | villagers namelist
│   │   ├── shops           | shops
│   │   ├── villagers       | don't know
│   │   ├── villages        | contains villages configuration files
│   │   └── walls           | contains walls related things
├── goals | contains all goals for every culture / villagers !
│   ├── genericcooking
│   ├── genericcrafting
│   ├── genericgatherblocks
│   ├── genericharvesting
│   ├── genericmining
│   ├── genericplanting
│   ├── genericplantsapling
│   ├── genericslaughteranimal
│   ├── generictakefrombuilding
│   ├── generictendfurnace
│   └── genericvisit
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
├── config-server.txt
├── config.txt
├── Content creation readme.txt
├── hof.txt
├── itemlist.txt
├── version.txt
└── WARNING - changes here will be overwritten on update.txt

```



### Deployment
When you install Millénaire for the first time, it deploys all its cultures data and settings in '/mods/millénaire' AND '/mods/millenaire-custom'.

#### folder '/mods/millénaire'
"The millenaire/ directory is auto-deployed by Millénaire on each new version of the mod, erasing all changes made to it.
This folder contains all the base files of every cultures, again it's all really human readable plain text, it will help when creating a culture

#### folder '/mods/millénaire-custom'
It's here that you will add things !


