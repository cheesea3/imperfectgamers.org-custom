***Imperfect Gamers***

# Custom Modular Plugins
>This repository includes the scripting / translation files for the imperfectgamers.org as well as the includes of Influx that they were compiled with. Only time Influx will get in the way is when the forwards change.
- When installing an update of influx, you'll have to remove one plugin if they are present: influx_simpleranks.
- influx_simpleranks should be kept on the server but needs convar influx_simpleranks_useclantag 0 so it doesn't interfere with the VIP scoreboard titles.

Most of these features were decoupled from the modified surftimer by SonicSNES, more information here: https://github.com/imperfectgamers/Surftimer
Part of this process involved the creation of a migration script, will add and update readme tomorrow with it included with steps.

## Features

> Each feature is broken up into components

- [Point Check](#points)
- [Records](#records)
- [Reports](#reports)
- [VIP](#vip)
---

## Points
> Configurable point check for skill server. Check client timer points on connect, if they don't have more than a configurable point count, they will be kicked from the server.  If set to 0, all clients can join.
>> *cvar on the test server is ig_pointcheck_min, defaults to 0*
    - 🍴 Check client timer points on connect
    - 🍴 If they don't have more than a configurable point count, they will be kicked from the server. 
    - 🍴 If set to 0, all clients can join.

## Records
> Configurable point check for skill server. Check client timer points on connect, if they don't have more than a configurable point count, they will be kicked from the server.  If set to 0, all clients can join.
    - 🍴 ig_records_webhook_announce is the records webhook convar
## Reports
> Allows players to be proactive in documenting important information for us. Gives us something to work with and reference.
    - 🍴 ig_reports_webhook_bugs !bugs menu (discord)
    - 🍴 ig_reports_webhook_calladmin !calladmin -> message (discord)
## Vip
> Notes about VIP.
    - 🍴 VIP Vote Extend cvar: ig_chat_prefix
    - 🍴 Color is formatting available {colourname} 
    - 🍴 !vmute is hooked with sourcebans and is logged to prevent abuse
    - 🍴 !ve runs ExtendMapTimeLimit(600) if vote is passed. Only allowed to initiate the last 5 minutes of timeleft.
    - 🍴 ?!title opens up a menu allowing VIP to cycle through their titles and change their name and text color seperately.
    


---
> Credits
SonicSNES - Custom features and modifications to Surftimer for imperfectgamers.org

- <a href="https://imperfectgamers.org"><img src="https://cdn.imperfectgamers.org/inc/assets/img/textlogo.png" width="15" height="15" title="Imperfect Gamers" alt="Logo"></a> Copyright 2020 © <a href="https://imperfectgamers.org" target="_blank">Imperfect Gamers</a>.
