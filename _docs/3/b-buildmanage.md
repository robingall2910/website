---
layout: docs
title: 3b. Build management
permalink: /docs/3/b-buildmanage/
---
As an admin, you are given powerful tools to manage block placements, deletions, and WorldEdit selections.
Learning to master these tools is important when rolling back grief and restoring other member's builds.

## Using CoreProtect
CoreProtect is a heavy block management tool that provides detailed logs of all blocks placed and removed.
This plugin allows you to make detailed, specific rollbacks and restorations while managing the integrity of our worlds.
You can display an in-gamel list of the available commands with three aliases:
 * `/coreprotect help` - The default and longest command, only admins can use it.
 * `/core help` - An alias of the default command, only admins can use it.
 * `/co help` - The shortest alias, only admins can use it.
<br>
We will demonstrate command usage with the alias `/co`, as it is the shortest and quickest, but all three variants are functional. 

### Block inspection tool
The inspection tool is a toggleable feature that allows you to left-click a block and view all previous changes made to that specific location.
It will show WorldEdit selections, placements, deletions, and even natrual changes such as water or an explosion.
 * `/co inspect` - Toggles the inspector and can be disabled by typing the command a second time.
 * `/co i` - An alias of the previous command and serves the same function.
<br>
This tool is mostly used to quickly check for damage such as a deleted build and also displays how long ago a change was made.

### Rolling back a member
Likely the most used tool of this plugin, the rollback feature allows an administrator to roll any member's changes back.
This command will affect just about anything so specifying parameters is important.
 * `/co rollback` - Preforms a rollback depending on the user and time you specify.
 * `/co rb` - An alias of the previous command and serves the same function.
<br>
#### Command usage
 * `/co rollback u:<user> t:<time> r:<radius> a:<action> b:<blocks> e:<exclude>`
 * `/co rb u:<user> t:<time> r:<radius> a:<action> b:<blocks> e:<exclude>`
 
The first three parameters should be used at all times, while the latter (action, blocks, exclude) are optional.
 * `u:<user>` - Specifies a member by their username to rollback.
 * `t:<time>` - Specifies the amount of time to roll a person back.
   <br>
   You can specify weeks (example, `t:1w`), days (`t:2d`), hours (`t:4h`), minutes (`t:10m`), or seconds (`t:5s`).
   <br>
   To be even more specific, you can pick time amounts (example, `t:1d4h`) and use decimals (`t:2.50h`).
 * `r:<radius>` - Specifies a radius, used to only rollback blocks near your location.
   <br>
   You can specify a number (example, `r:5`), a world (`r:flatlands`), or a global rollback (`r:global`).
