# BETA

# Velocity-Skript



### _**A Velocity Plugin where you can create your own commands like the bukkit plugin Skript!**_

![Ingame](https://cdn.modrinth.com/data/cached_images/a149a4d9e43404996cbc4703932cb447d1590e0c.png)






**Test.vsk**  _(every skript file need to end with .vsk to work)_
```
# Welcome message on player join
on join:
    send "Welcome, %player%! Enjoy your stay on %players-server%!" to player

# Commands
command /greet:
    trigger:
        send "Hello, %player%! Welcome to the server!" to player

# Broadcast to the everybody
command /broadcast:
    trigger:
        broadcast "Attention everyone!"

command /connectlobby:
    trigger:
        connect player to "Lobby-1"
```


## Available Placeholders

> **%player%**
> 
> Description: This placeholder is replaced with the username of the player who triggered the command or event.
> Example Usage: send "Hello, %player%!" to player
> Example Output: Hello, DieSuperKatze!


> **%players-server%**
> 
> Description: This placeholder is replaced with the name of the server that the player is currently connected to.
> Example Usage: send "You are currently on %players-server%." to player
> Example Output: You are currently on Lobby-1.


> **%loop-player%**
> 
> Description: This placeholder is used within a loop of all players. It is replaced with the username of the player being processed in the current iteration of the loop.
> Example Usage: send "Hello, %loop-player%!" to loop-player
> Example Output: Hello, Player1! (and so on for each player in the loop)




## Todo:

- Adding events for setting Server Motds
- Adding multiple arguments in one command
- Fix issues with the every <time> event
