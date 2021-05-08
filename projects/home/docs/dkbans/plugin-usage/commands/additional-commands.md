---
title: Additional Commands
---

# Additional Commands

This page describes the usage and permissions of the DKCoins general commands.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/joinme```](#joinme)
* [```/chatClear [local/global]```](#chatclear-localglobal)
* [```/teamChat <login/logout/toggle/message>```](#teamchat-loginlogouttogglemessage)
* [```/chatlog player <player>```](#chatlog-player-player)
* [```/chatlog server <server>```](#chatlog-server-server)
* [```/notify <login/logout/toggle>```](#notify-loginlogouttoggle)
* [```/punishNotify <login/logout/toggle>```](#punishnotify-loginlogouttoggle)
* [```/help```](#help)

***

## **```/joinme```**

**Permission:** dkbans.joinme<br />

Send a global joinme message to all online players. Other players can then connect to the same server.

***

## **```/chatClear [local/global]```**

**Alias:** ccheat, cc <br/>
**Permission:** 
  * dkbans.command.chatclear (Allows to clear the own chat)
  * dkbans.chatClear.all (Allows to clear global and local chat)
**Arguments:**
* `local` Clear the chat for all players on the current server
* `global` Clear the chat for all players on the entire network

Clear the own, local or global chat.

***

## **```/teamChat <login/logout/toggle/message>```**

**Alias:** tchat, tc <br/>
**Permission:**
  * dkbans.teamchat.receive (Receive team chat messages)
  * dkbans.teamchat.send (Send team chat messages)
**Arguments:**
* `login` Login to the team chat
* `logout` Logout from the team chat
* `toggle` Toggle the login/logout status
* `<message>` Send a message to the team chat

Used to communicate in game with all team members.

***

## **```/chatlog player <player>```**

**Permission:** dkbans.command.chatlog<br/>
**Arguments:**
* `player <player>` The name of the player

Get the chat log of a player.

***

## **```/chatlog server <server>```**

**Permission:** dkbans.command.chatlog<br/>
**Arguments:**
* `server <server>` The name of the server

Get the chat log of a server.

***

## **```/punishNotify <login/logout/toggle>```**

**Permission:** dkbans.punish.notify<br/>
**Arguments:**
* `login` Login to the receive messages
* `logout` Logout to ignore messages
* `toggle` Toggle the login/logout status

Login to receive punishment notifications.

***

## **```/notify <login/logout/toggle>```**

**Permission:** dkbans.punish.notify<br/>
**Arguments:**
* `login` Login to the receive messages
* `logout` Logout to ignore messages
* `toggle` Toggle the login/logout status

Logout/Login from all channels (report, punishments, team chat).

***

## **```/help```**

A global help message for your players (configurable in the messages).

***
