# Minecraft Fishing Bot

Minecraft fishing bot made using [Mineflayer](https://github.com/PrismarineJS/mineflayer)

## What it can do

1. Navigate to a fishing spot
2. Send chat message on what it caught
3. Store items in a nearby chest
4. Sleep when it is night (Only if there are unoccupied beds)
5. Go to you, or an (x, y, z) coordinate

## How to use

To start the bot, the bot must be run with these arguments:

`node fisherman.js <prefix> <host> <port> <name> [<password>] [<viewer_port>]`

`prefix`: the prefix to call your bot.

`host`: the IP of the server you want the bot to connect to (can be localhost).

`port`: the port of the server you want the bot to connect to.

`name`: username to log in to minecraft (can be anything if joining an offline-mode server)

`password`(optional): optional if joining a offline-mode server. Password to the minecraft account.

`viewer_port`(optional): Port for the viewer. If unset, viewer won't start.

## Commands

### start

```
<prefix> start <y_offset>
```

Goes to the closest body of water and starts fishing. `<y_offset>` determines how high the fishermen will aim from the initial water block coordinates.

### stop

```
<prefix> stop
```

Stops fishing.

### sleep

```
<prefix> sleep
```

Tries to force the fishermen to sleep. They usually sleep automatically.

### nearwater

```
<prefix> nearwater
```

Makes the fishermen go near water. Nothing more, nothing less.

### goto

```
<prefix> goto <player>|<x y z>
```

`<player>` can be a player name or `me` if you want the bot to go to you.

### store

```
<prefix> store [all]
```

Goes to the closest chest and stores the items fished. Add `all` argument to store even the fishing rods.

### follow

```
<prefix> follow <player>
```

Specifies `<player>` to follow.

### unfollow

```
<prefix> unfollow
```

Unfollows players.

### rc

```
<prefix> rc
```

Makes the fishermen perform a right click.

## Images

![fishing](https://i.imgur.com/aHArRgO.png)

![storing](https://i.imgur.com/DLDErYJ.png)
