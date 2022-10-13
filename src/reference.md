# Command Reference

IgKnite currentry has a total of 37 available bot commands, roughly distributed among four categories. All the commands are built on Discord's bleeding edge API and use the latest features.

The following is a list of all the available commands (updated: October 13, 2022).

## The Customization Commands
### /makerole [name]
Creates a new server role with the specified *name*.

### /assignrole [member] [role]
Assigns a server *role* to the specified *member*.

### /removerole [role]
Removes a *role* from the server.

### /makeinvite [max_age] [max_uses] [reason]
Creates an invitation link to the server with the specified parameters.

| Parameter | Required | Default |
|---|---|---|
| max_age | No | 0 |
| max_uses | No | 1 |
| reason | No | No reason provided. |

### /nick [member] [nickname]
Changes the server *nickname* of the specified *member*

### /makechannel [name] [category] [topic]
Creates a new channel in the server with the given *name*, inside the given *category*, and sets the given *topic* to it.

| Parameter | Required | Default |
|---|---|---|
| name | Yes |  |
| category | No | None |
| topic | No | None |

### /makevc [name] [category]
Creates a new voice channel with the given *name* in the given *category*.

| Parameter | Required | Default |
|---|---|---|
| name | Yes |  |
| category | No | None |

### /makecategory [name]
Creates a new channel category with the specified *name*.

### /removechannel [channel]
Deletes the given *channel* from the server.

### /reset
Deletes all the messages from the current channel.


## The General Commands
### /avatar [member]
Displays your avatar or the avatar of the server *member* given.

| Parameter | Required | Default |
|---|---|---|
| member | No | You |

### /ping
Returns IgKnite's API response time, system latency, and uptime.


## The Moderation Commands
### /ban [member] [reason]
Bans the given server *member* for the given *reason*.

| Parameter | Required | Default |
|---|---|---|
| member | Yes |  |
| reason | No | No reason provided |

### /unban [member]
Unbans the given *member* from the server.

### /softban [member] [reason]
Temporarily bans the given *member* to delete their messages.

| Parameter | Required | Default |
|---|---|---|
| member | Yes |  |
| reason | No | No reason provided |

### /kick [member] [reason]
Kicks the given *member* from the server.

*Note: Kicked members can join the server again, but banned members can't.*

| Parameter | Required | Default |
|---|---|---|
| member | Yes |  |
| reason | No | No reason provided |

### /timeout [member] [duration] [reason]
Timeouts the given *member*.

| Parameter | Required | Default |
|---|---|---|
| member | Yes |  |
| duration | No | 30 seconds |
| reason | No | No reason provided |

### /purge [amount]
Deletes the given *number/amount* of messages in the channel.

| Parameter | Required | Default |
|---|---|---|
| amount | No | 1 |

### /ripplepurge [member] [amount]
Clears the messages sent by the given *member* if they fall in the given *index/amount*.

### /snipe
Recovers all the messages that were deleted/*sniped* in the last 25 seconds. *Neat, right?*

### /senddm [member] [msg]
Sends a message to the specified member's DM.

| Parameter | Required | Default |
|---|---|---|
| member | Yes | None|
| msg | Yes | None|

## The Inspection Commands
### /guildinfo
Shows all important information about the server.

![/guildinfo demonstration](static/dem_guildinfo.png)

### /userinfo [member]
Shows all important information on a user.

| Parameter | Required | Default |
|---|---|---|
| member | No | You |

![/userinfo demonstration](static/dem_userinfo.png)

### /roleinfo [role]
Shows all important information related to a specific role.

![/roleinfo demonstration](static/dem_roleinfo.png)

## The Music Commands
### /play [keyword]
Searches a soundtrack with the given *keyword* and adds it to the queue.

![/play demonstration](static/dem_play.png)

### /pause
Pauses the currently playing song.

### /resume
Resumes the currently playing song.

### /stop
Stops playing the song and clears the queue.

### /join
Joins the VC you are in.

### /leave
Leaves the VC you are in (duh?).

### /volume [volume]
Sets the volume of the playing song. Just say `/volume 50`.

### /now
Displays an interactive control view for the current song.

![/now demonstration](static/dem_now.png)

### /skip
Vote to skip a song. The requester can automatically skip.

### /queue
Shows the player's queue.

![/queue demonstration](static/dem_queue.png)

### /rmqueue [index]
Removes a song from the queue at a given *index*.