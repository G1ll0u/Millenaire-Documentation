# Millenaire-documentation
## WIP documentation about our good old Millénaire 1.12.2 mod

This documentation  is mainly focused on controlled villages and custom controlled villages.

## Who should read that ?
People that already know Millénaire and want to customize it.

## why you do that bro ?
Because that's my favorite mod of all times.
I'm not a developer, I just take advantage of how good this mod is made because every file that helps customize the mod are simple plain text files.
You can do all sort of customization like :
Create or edit goals that are followed by villagers (like harvest wood)
Create or edit entire cultures
Create new villagers

By the way, check out my addon that tweaks existing cultures: https://github.com/G1ll0u/Millenaire-fixes/

## What is Millénaire ?
Millénaire is an old Minecraft mod that adds villages and reputation or quests in Minecraft (1.12.2 currently). By default, the mod generates villages like Minecraft do for normal villagers. Every villager has a role and goals assigned, you can also create your own village assign every building to villagers. Every villager has a role and goals assigned to this role and you can customize a lot of things here.

There are normal villages, controlled villages and custom controlled villages :

## Normal villages
It generates when you discover the world, you can interact with it by doing quests and trading. They will need resources to build new buildings or upgrade existing ones. 

## Controlled villages
When your reputation is high enough for a specific culture, you will be able, when talking to the boss of this culture village, to request to be a chief of this culture. Being a chief allows you to create controlled villages where YOU are the boss. 

Controlled village is simply a village that you generate where you want by using the wand of creation on a golden block. There will be no chief villager because YOU are the chgief and you can order villagers to create buildings at specific places with your wand.

### Custom controlled villages

Custom controlled villages are normal villages but it lets you create a custom village centre (townhall). It makes you spawn 3 male and 3 female teenagers, that will grow up in the houses you assign to them that you built yourself or ordered them to build.

## Introduction to how Millénaire cultures work
The principle of millénaire is that you have cultures :
**byzantines**  **indian**  **inuits**  **japanese**  **mayan**  **norman**  **seljuk**

I will focus on normans because it's the most complete culture.

Every culture has villagers, here are some :
**farmer wife boy girl**

Every villagers have goals here are some :
**makeBread plantWheat harvestWheat childEatApples goDrinkCider**

Their housing :
**armoury bakery quarry**

You can play with all these aspects by simply manipulating txt files.

### Deployment
When you install Millénaire for the first time, it deploys all its cultures data and settings in '/mods/millénaire' AND '/mods/millenaire-custom'.

#### folder /mods/millénaire
"The /mods/millenaire/ directory is auto-deployed by Millénaire. **Be careful, updating the mod erases all changes made to this directory.**
This folder contains all the base files of every cultures, again it's all really human readable plain text, it will help when creating a culture.

Do not edit any of these txt files 

#### folder '/mods/millénaire-custom'
It's here that you will add things !
in '/mods/millénaire-custom/mods', you can create folders and each folder will be loaded by Millénaire as an add-on. 


## Files and directory structures with some explanations
Here is the directory tree of /mods/millénaire with simple explanations :

```
├──────────────────────────────────────────────────────────────────────────────────────────────────────────
/millenaire
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
├── goals             | contains all goals for every culture / villagers !
│   ├── genericcooking      | cooking goals
│   ├── genericcrafting     | crafting goals
│   ├── genericgatherblocks | etc.
│   ├── genericharvesting 
│   ├── genericmining
│   ├── genericplanting
│   ├── genericplantsapling
│   ├── genericslaughteranimal
│   ├── generictakefrombuilding 
│   ├── generictendfurnace
│   └── genericvisit        | goals like "goDrinkCider
├── help             | helpful documentation
├── languages        | contains all strings of text, I didn't try for the moment but I think that when you create custom
goals, you can edit what text that will be shown above the villager when he does this goal.
│ 
├── quests           | quests related stuff
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
└── villagerconfig     | how villagers will behave about items (what sword type should I take in priority ?)
I think you can add modded items 
├── blocklist.txt 
├── blocktypes.txt     | Allows to whitelist/blacklist blocks so they can build or spawn on it (can be useful when encountering
problems with other mods)
├── Colour Sheet.png
├── config-server.txt  | default server config file
├── config.txt         | default client config file
├── hof.txt            | hall of fame
├── itemlist.txt       | list of items
├── version.txt        | Don't touch it
├────────────────────────────────────────────────────────────────────────────────────────────────────────────
```

