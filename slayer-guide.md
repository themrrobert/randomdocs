**__Using Cannon/Burst/Barrage__**
You're minion can now use a cannon, and burst or barrage tasks!
To get started, you'll need a cannon. Hope you have 10 mil!
```
+buy dwarf multicannon
```
Killing monsters with the cannon:
```
+k dagannoth --cannon
```
Any monster that can be killed in multi WILL be killed in multi, you cannot choose. Single way combat cannon usage has a lower cannonball cost, but also a lower boost.

Abby demons can also be killed with barrage. This uses a fair bit of runes, so you can also use `+k abby demons --burst` if you're on a budget:
```
+k abby demons --burst
```
You can also use the --barrage/--burst/--cannon flags with +autoslay:
```
+as default --cannon
``` 
But you will probably want to be more specific and use the `+k` command if you aren't sure what you're going to get. 
**Just like always there is no confirmation for PVM trips, **
and cancelling the trip will sacrifice the supplies used to start the trip, including cannonballs or runes!

You can tell your minion to always use a cannon and/or burst/barrage with:
```
+combatoptions help
+cbops add cannon 
+cbops remove burst
```
You can set EITHER burst or barrage (setting the barrage will un-set burst, for example), but you can also enable the cannon as well.
If you have both a burst or barrage spell AND cannon enabled, then burst/barrage will take priority if both options are available.

**__Commands:__**
```
+slayertask  |  +st
+slayershop
+autoslay  |  +as  |  +slay
```

**__Getting Tasks:__**
Get a new slayer task from Konar:
```
+slayertask konar
```
Get a new task from duradel, and saves duradel as the default slayer master:
```
+slayertask duradel --save
```
Get's a new slayer task from the default [saved] slayer master:
```
+st
```
Skips the current task without confirmation. Costs 30 slayer points, but does not reset streak:
```
+st --skip --cf
```
Skips the current task BUT will reset your streak. Free, but you can only skip tasks Turael doesn't provide:
```
+st turael
```
Forgets the current default slayer master:
```
+st --forget
```

**__Killing Monsters__**
You can kill slayer monsters with the +k command as always, but now you can do:
Automatically kills the greatest number possible of the default slayer creature in the category. 
The word default is in brackets [] because it's the default choice, you don't need to type the brackets.
```
+autoslay [default]
```
This automatically kills the boss variant of the slayer task, or if one doesn't exist, the objectively 'best' monster of the category:
```
Autoslay now supports 'ehp' aka 'efficient' mode, which will use the most efficient method available. 
However, if you don't have the requirements, you will get an error and have to +k manually.
This is to prevent doing a task you didn't mean to do.
```
+autoslay ehp --save
+as
```
+autoslay boss
```
You can use the --save flag with +autoslay to make that option the new default.
Reset the default behavior of autoslay:
```
+as default --save
```
'lowest' is an alias for 'default', and 'highest' is an alias for 'boss.' They don't necessarily mean strictly the lowest/higher combat combat, they are just there for convenience.

Cannon dagannoths in the lighthouse if Dagannoth is your slayer task:
```
+as default --cannon
```

**__Unlocking Rewards__**
Show which rewards you have unlocked:
```
+slayershop
```
Offers to buy the Slayer helm create unlock for 400 points:
```
+slayershop unlock malevolent masquerade
```
```
+sls unlock slayer helmet
```
Buys without confirmation the abyssal slayer helmet unlock.
```
+slayershop unlock red slayer helmet --cf
```
Re-locks red dragons. Use this if you want to un-extend or otherwise remove a toggle-able unlock:
**You will have to spend points again to unlock it if you choose.** 
```
+sls lock seeing red
```
You can use the official Unlock name, like unholy helmet, or common alises work as well.
COLOR slayer helmet should work. 

So will the names of the slayer creature to unlock.

**__Example:__**
Instead of:
```
+slayershop unlock Seeing Red
```
You can do:
```
+slayershop unlock red dragons
```
         
**__Blocking Tasks__**
If you want to block a task, it costs 100 slayer poitns.
You get 1 block slot for free, then 1 more for each 50 qps up to 6 slots at 250.
--cf will confirm automatically.
```
+st --block --cf
```
Show all of your blocked tasks:
```
+st --list
```
Unblocks blue dragons task:
```
+st --unblock blue dragon
```

**__Creating Slayer Items__**
Creates slayer helmet, you need the ingredients, buyable from bot, except Black mask.
You also need 55 crafting:
```
+create slayer helmet
```
Creates a slayer ring (8) from a gold bar and an enchanted gem (also buyable)
```
+create slayer ring (8)
```
Does what it says on the tin:
```
+create slayer ring (eternal)
+create abyssal bludgeon
```

**__Miscellaneous__**
This will offer ALL of your Unsired to the Font of consumption, or just 1 if you specify:
```
+offer unsired
+offer 1 unsired
```
