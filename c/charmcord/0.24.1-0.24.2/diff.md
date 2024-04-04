# Comparing `tmp/charmcord-0.24.1.tar.gz` & `tmp/charmcord-0.24.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charmcord-0.24.1.tar", max compression
+gzip compressed data, was "charmcord-0.24.2.tar", max compression
```

## Comparing `charmcord-0.24.1.tar` & `charmcord-0.24.2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0      333 2024-03-14 06:59:51.324104 charmcord-0.24.1/CharmCord/__init__.py
--rw-r--r--   0        0        0     1739 2024-04-03 15:34:15.303034 charmcord-0.24.1/CharmCord/all_functions.py
--rw-r--r--   0        0        0      686 2024-03-09 17:02:01.479681 charmcord-0.24.1/CharmCord/CharmErrorHandling.py
--rw-r--r--   0        0        0      268 2024-04-04 00:06:53.266312 charmcord-0.24.1/CharmCord/functions/__init__.py
--rw-r--r--   0        0        0      403 2024-04-03 19:16:50.219032 charmcord-0.24.1/CharmCord/functions/Channels/__init__.py
--rw-r--r--   0        0        0      562 2024-04-04 07:14:11.909221 charmcord-0.24.1/CharmCord/functions/Channels/channelCategoryID.py
--rw-r--r--   0        0        0      675 2024-04-04 07:14:11.829435 charmcord-0.24.1/CharmCord/functions/Channels/channelCategoryName.py
--rw-r--r--   0        0        0      982 2024-04-04 07:14:11.842399 charmcord-0.24.1/CharmCord/functions/Channels/channelChangedRoles.py
--rw-r--r--   0        0        0     1217 2024-04-04 07:14:11.930165 charmcord-0.24.1/CharmCord/functions/Channels/channelCreated.py
--rw-r--r--   0        0        0      634 2024-04-04 07:14:11.914208 charmcord-0.24.1/CharmCord/functions/Channels/channelDelay.py
--rw-r--r--   0        0        0      156 2024-03-09 17:02:01.485625 charmcord-0.24.1/CharmCord/functions/Channels/channelID.py
--rw-r--r--   0        0        0      633 2024-04-04 07:14:11.861349 charmcord-0.24.1/CharmCord/functions/Channels/channelMention.py
--rw-r--r--   0        0        0      609 2024-04-04 07:14:11.936150 charmcord-0.24.1/CharmCord/functions/Channels/channelName.py
--rw-r--r--   0        0        0      647 2024-04-04 07:14:11.944127 charmcord-0.24.1/CharmCord/functions/Channels/channelNsfw.py
--rw-r--r--   0        0        0      635 2024-04-04 07:14:11.883324 charmcord-0.24.1/CharmCord/functions/Channels/channelPosition.py
--rw-r--r--   0        0        0      613 2024-04-04 07:14:11.888278 charmcord-0.24.1/CharmCord/functions/Channels/channelType.py
--rw-r--r--   0        0        0      601 2024-04-04 07:14:11.895258 charmcord-0.24.1/CharmCord/functions/Channels/channelURL.py
--rw-r--r--   0        0        0       51 2024-04-03 19:05:05.886849 charmcord-0.24.1/CharmCord/functions/Channels/threadAutoArchive.py
--rw-r--r--   0        0        0      405 2024-04-03 19:16:50.193021 charmcord-0.24.1/CharmCord/functions/Client/__init__.py
--rw-r--r--   0        0        0      151 2024-04-04 07:14:11.848384 charmcord-0.24.1/CharmCord/functions/Client/botAvatar.py
--rw-r--r--   0        0        0      142 2024-04-04 07:14:11.949114 charmcord-0.24.1/CharmCord/functions/Client/botGuilds.py
--rw-r--r--   0        0        0      137 2024-04-04 07:14:11.870328 charmcord-0.24.1/CharmCord/functions/Client/botID.py
--rw-r--r--   0        0        0      149 2024-04-04 07:14:11.854368 charmcord-0.24.1/CharmCord/functions/Client/botMention.py
--rw-r--r--   0        0        0      143 2024-04-04 07:14:11.902241 charmcord-0.24.1/CharmCord/functions/Client/botName.py
--rw-r--r--   0        0        0      154 2024-04-04 07:14:11.877306 charmcord-0.24.1/CharmCord/functions/Client/ping.py
--rw-r--r--   0        0        0     1223 2024-03-09 17:02:01.522527 charmcord-0.24.1/CharmCord/functions/clientActivity.py
--rw-r--r--   0        0        0      403 2024-04-03 19:16:50.224079 charmcord-0.24.1/CharmCord/functions/Events/__init__.py
--rw-r--r--   0        0        0     1367 2024-03-12 15:03:01.233500 charmcord-0.24.1/CharmCord/functions/Events/_options_.py
--rw-r--r--   0        0        0      171 2024-04-03 19:17:35.455552 charmcord-0.24.1/CharmCord/functions/Events/deletedChannel.py
--rw-r--r--   0        0        0      167 2024-04-03 19:17:35.451468 charmcord-0.24.1/CharmCord/functions/Events/memberJoined.py
--rw-r--r--   0        0        0      163 2024-04-03 19:17:35.444186 charmcord-0.24.1/CharmCord/functions/Events/newChannel.py
--rw-r--r--   0        0        0      163 2024-04-03 19:17:35.460722 charmcord-0.24.1/CharmCord/functions/Events/oldChannel.py
--rw-r--r--   0        0        0      169 2024-04-03 19:16:50.198158 charmcord-0.24.1/CharmCord/functions/Events/reactionAdded.py
--rw-r--r--   0        0        0      171 2024-04-03 19:16:50.208493 charmcord-0.24.1/CharmCord/functions/Events/reactionRemoved.py
--rw-r--r--   0        0        0      403 2024-04-03 19:16:50.234419 charmcord-0.24.1/CharmCord/functions/Guilds/__init__.py
--rw-r--r--   0        0        0      229 2024-03-09 17:02:01.497593 charmcord-0.24.1/CharmCord/functions/Guilds/guildID.py
--rw-r--r--   0        0        0      450 2024-04-04 07:08:16.543821 charmcord-0.24.1/CharmCord/functions/Guilds/guildName.py
--rw-r--r--   0        0        0      599 2024-04-04 07:10:02.301739 charmcord-0.24.1/CharmCord/functions/Guilds/guildTextChannels.py
--rw-r--r--   0        0        0      403 2024-04-03 19:11:35.344498 charmcord-0.24.1/CharmCord/functions/Messages/__init__.py
--rw-r--r--   0        0        0       25 2024-04-03 17:45:00.065444 charmcord-0.24.1/CharmCord/functions/Messages/_btnOpts_.py
--rw-r--r--   0        0        0     2473 2024-04-04 06:49:04.962972 charmcord-0.24.1/CharmCord/functions/Messages/addButton.py
--rw-r--r--   0        0        0      559 2024-04-03 19:16:50.250927 charmcord-0.24.1/CharmCord/functions/Messages/buttonSend.py
--rw-r--r--   0        0        0      346 2024-03-09 17:02:01.499587 charmcord-0.24.1/CharmCord/functions/Messages/defer.py
--rw-r--r--   0        0        0      455 2024-03-09 17:02:01.500584 charmcord-0.24.1/CharmCord/functions/Messages/deleteMessage.py
--rw-r--r--   0        0        0      735 2024-03-09 17:02:01.500584 charmcord-0.24.1/CharmCord/functions/Messages/editMessage.py
--rw-r--r--   0        0        0      300 2024-03-09 17:02:01.501582 charmcord-0.24.1/CharmCord/functions/Messages/mentions.py
--rw-r--r--   0        0        0      394 2024-04-04 06:54:00.774631 charmcord-0.24.1/CharmCord/functions/Messages/message.py
--rw-r--r--   0        0        0      388 2024-04-04 06:54:00.767650 charmcord-0.24.1/CharmCord/functions/Messages/messageAuthor.py
--rw-r--r--   0        0        0      390 2024-04-04 06:54:00.781639 charmcord-0.24.1/CharmCord/functions/Messages/messageContent.py
--rw-r--r--   0        0        0       67 2024-03-09 17:02:01.502579 charmcord-0.24.1/CharmCord/functions/Messages/messageID.py
--rw-r--r--   0        0        0      392 2024-04-04 06:54:00.755682 charmcord-0.24.1/CharmCord/functions/Messages/messageMentions.py
--rw-r--r--   0        0        0     1544 2024-04-04 00:08:30.208461 charmcord-0.24.1/CharmCord/functions/Messages/purge.py
--rw-r--r--   0        0        0     2316 2024-04-04 00:07:36.109871 charmcord-0.24.1/CharmCord/functions/Messages/sendEmbed.py
--rw-r--r--   0        0        0      997 2024-04-04 00:06:53.255340 charmcord-0.24.1/CharmCord/functions/Messages/sendMessage.py
--rw-r--r--   0        0        0      469 2024-03-09 17:02:01.504574 charmcord-0.24.1/CharmCord/functions/Messages/slashSend.py
--rw-r--r--   0        0        0     1424 2024-04-04 06:54:00.789640 charmcord-0.24.1/CharmCord/functions/Messages/waitMessage.py
--rw-r--r--   0        0        0     1697 2024-03-09 17:02:01.505571 charmcord-0.24.1/CharmCord/functions/Messages/waitReaction.py
--rw-r--r--   0        0        0      403 2024-04-03 19:16:50.229203 charmcord-0.24.1/CharmCord/functions/Python/__init__.py
--rw-r--r--   0        0        0     1035 2024-03-09 17:02:01.508563 charmcord-0.24.1/CharmCord/functions/Python/charmAI.py
--rw-r--r--   0        0        0       64 2024-03-09 17:02:01.508563 charmcord-0.24.1/CharmCord/functions/Python/console.py
--rw-r--r--   0        0        0      278 2024-03-09 17:02:01.509560 charmcord-0.24.1/CharmCord/functions/Python/count.py
--rw-r--r--   0        0        0      581 2024-03-11 09:10:42.723633 charmcord-0.24.1/CharmCord/functions/Python/divide.py
--rw-r--r--   0        0        0      854 2024-03-09 17:02:01.506569 charmcord-0.24.1/CharmCord/functions/Python/ElIf.py
--rw-r--r--   0        0        0      779 2024-03-09 17:02:01.509560 charmcord-0.24.1/CharmCord/functions/Python/getJson.py
--rw-r--r--   0        0        0      852 2024-03-09 17:02:01.507566 charmcord-0.24.1/CharmCord/functions/Python/If.py
--rw-r--r--   0        0        0      577 2024-03-11 05:59:49.520543 charmcord-0.24.1/CharmCord/functions/Python/multi.py
--rw-r--r--   0        0        0     1955 2024-03-09 17:02:01.511594 charmcord-0.24.1/CharmCord/functions/Python/onlyIf.py
--rw-r--r--   0        0        0       78 2024-03-10 20:37:06.628081 charmcord-0.24.1/CharmCord/functions/Python/pyEval.py
--rw-r--r--   0        0        0      569 2024-03-11 09:10:42.717522 charmcord-0.24.1/CharmCord/functions/Python/sub.py
--rw-r--r--   0        0        0      571 2024-03-09 17:02:01.512553 charmcord-0.24.1/CharmCord/functions/Python/sum.py
--rw-r--r--   0        0        0      101 2024-03-09 17:02:01.512553 charmcord-0.24.1/CharmCord/functions/Python/wait.py
--rw-r--r--   0        0        0      403 2024-04-03 19:16:50.187749 charmcord-0.24.1/CharmCord/functions/Users/__init__.py
--rw-r--r--   0        0        0      182 2024-03-09 17:02:01.513550 charmcord-0.24.1/CharmCord/functions/Users/authorID.py
--rw-r--r--   0        0        0      188 2024-03-09 17:02:01.514547 charmcord-0.24.1/CharmCord/functions/Users/authorName.py
--rw-r--r--   0        0        0      355 2024-03-09 17:02:01.514547 charmcord-0.24.1/CharmCord/functions/Users/hasPerm.py
--rw-r--r--   0        0        0      481 2024-04-04 07:04:39.105167 charmcord-0.24.1/CharmCord/functions/Users/sendDM.py
--rw-r--r--   0        0        0      428 2024-04-04 07:08:16.560775 charmcord-0.24.1/CharmCord/functions/Users/userID.py
--rw-r--r--   0        0        0      440 2024-04-04 07:08:16.572742 charmcord-0.24.1/CharmCord/functions/Users/userMention.py
--rw-r--r--   0        0        0      434 2024-04-04 07:04:39.117135 charmcord-0.24.1/CharmCord/functions/Users/userName.py
--rw-r--r--   0        0        0      403 2024-04-03 19:16:50.244746 charmcord-0.24.1/CharmCord/functions/Variables/__init__.py
--rw-r--r--   0        0        0       92 2024-04-04 06:58:15.526257 charmcord-0.24.1/CharmCord/functions/Variables/get.py
--rw-r--r--   0        0        0      669 2024-04-04 07:00:42.664752 charmcord-0.24.1/CharmCord/functions/Variables/getServerVar.py
--rw-r--r--   0        0        0      751 2024-04-04 07:00:42.654806 charmcord-0.24.1/CharmCord/functions/Variables/getUserVar.py
--rw-r--r--   0        0        0      256 2024-03-09 17:02:01.519534 charmcord-0.24.1/CharmCord/functions/Variables/getVar.py
--rw-r--r--   0        0        0      174 2024-03-09 17:02:01.519534 charmcord-0.24.1/CharmCord/functions/Variables/let.py
--rw-r--r--   0        0        0      485 2024-03-09 17:02:01.520531 charmcord-0.24.1/CharmCord/functions/Variables/setServerVar.py
--rw-r--r--   0        0        0      556 2024-03-09 17:02:01.520531 charmcord-0.24.1/CharmCord/functions/Variables/setUserVar.py
--rw-r--r--   0        0        0      484 2024-03-09 17:02:01.521528 charmcord-0.24.1/CharmCord/functions/Variables/setVar.py
--rw-r--r--   0        0        0      477 2024-04-03 17:49:57.082699 charmcord-0.24.1/CharmCord/globeHandler.py
--rw-r--r--   0        0        0    13944 2024-04-04 07:22:05.334490 charmcord-0.24.1/CharmCord/tools.py
--rw-r--r--   0        0        0       65 2024-03-09 17:02:01.526515 charmcord-0.24.1/CharmCord/utils/__init__.py
--rw-r--r--   0        0        0     9945 2024-04-04 00:04:40.167585 charmcord-0.24.1/CharmCord/utils/CharmCord.py
--rw-r--r--   0        0        0     2515 2024-04-03 23:56:24.556283 charmcord-0.24.1/CharmCord/utils/Cogs.py
--rw-r--r--   0        0        0      352 2024-03-09 17:02:01.524520 charmcord-0.24.1/CharmCord/utils/CommandHandler.py
--rw-r--r--   0        0        0     1001 2024-04-03 23:59:12.759697 charmcord-0.24.1/CharmCord/utils/Commands.py
--rw-r--r--   0        0        0     2349 2024-04-03 23:53:40.730100 charmcord-0.24.1/CharmCord/utils/SlashCommands.py
--rw-r--r--   0        0        0    35823 2024-03-09 17:02:01.528510 charmcord-0.24.1/LICENSE
--rw-r--r--   0        0        0      914 2024-04-04 07:43:18.730757 charmcord-0.24.1/pyproject.toml
--rw-r--r--   0        0        0     3219 2024-04-04 07:42:59.033234 charmcord-0.24.1/README.md
--rw-r--r--   0        0        0     3809 1970-01-01 00:00:00.000000 charmcord-0.24.1/PKG-INFO
+-rw-r--r--   0        0        0      333 2024-03-14 06:59:51.324104 charmcord-0.24.2/CharmCord/__init__.py
+-rw-r--r--   0        0        0     1739 2024-04-03 15:34:15.303034 charmcord-0.24.2/CharmCord/all_functions.py
+-rw-r--r--   0        0        0      686 2024-03-09 17:02:01.479681 charmcord-0.24.2/CharmCord/CharmErrorHandling.py
+-rw-r--r--   0        0        0      268 2024-04-04 00:06:53.266312 charmcord-0.24.2/CharmCord/functions/__init__.py
+-rw-r--r--   0        0        0      403 2024-04-03 19:16:50.219032 charmcord-0.24.2/CharmCord/functions/Channels/__init__.py
+-rw-r--r--   0        0        0      562 2024-04-04 07:14:11.909221 charmcord-0.24.2/CharmCord/functions/Channels/channelCategoryID.py
+-rw-r--r--   0        0        0      675 2024-04-04 07:14:11.829435 charmcord-0.24.2/CharmCord/functions/Channels/channelCategoryName.py
+-rw-r--r--   0        0        0      982 2024-04-04 07:14:11.842399 charmcord-0.24.2/CharmCord/functions/Channels/channelChangedRoles.py
+-rw-r--r--   0        0        0     1217 2024-04-04 07:14:11.930165 charmcord-0.24.2/CharmCord/functions/Channels/channelCreated.py
+-rw-r--r--   0        0        0      634 2024-04-04 07:14:11.914208 charmcord-0.24.2/CharmCord/functions/Channels/channelDelay.py
+-rw-r--r--   0        0        0      156 2024-03-09 17:02:01.485625 charmcord-0.24.2/CharmCord/functions/Channels/channelID.py
+-rw-r--r--   0        0        0      633 2024-04-04 07:14:11.861349 charmcord-0.24.2/CharmCord/functions/Channels/channelMention.py
+-rw-r--r--   0        0        0      609 2024-04-04 07:14:11.936150 charmcord-0.24.2/CharmCord/functions/Channels/channelName.py
+-rw-r--r--   0        0        0      647 2024-04-04 07:14:11.944127 charmcord-0.24.2/CharmCord/functions/Channels/channelNsfw.py
+-rw-r--r--   0        0        0      635 2024-04-04 07:14:11.883324 charmcord-0.24.2/CharmCord/functions/Channels/channelPosition.py
+-rw-r--r--   0        0        0      613 2024-04-04 07:14:11.888278 charmcord-0.24.2/CharmCord/functions/Channels/channelType.py
+-rw-r--r--   0        0        0      601 2024-04-04 07:14:11.895258 charmcord-0.24.2/CharmCord/functions/Channels/channelURL.py
+-rw-r--r--   0        0        0       51 2024-04-03 19:05:05.886849 charmcord-0.24.2/CharmCord/functions/Channels/threadAutoArchive.py
+-rw-r--r--   0        0        0      405 2024-04-03 19:16:50.193021 charmcord-0.24.2/CharmCord/functions/Client/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-04 07:14:11.848384 charmcord-0.24.2/CharmCord/functions/Client/botAvatar.py
+-rw-r--r--   0        0        0      142 2024-04-04 07:14:11.949114 charmcord-0.24.2/CharmCord/functions/Client/botGuilds.py
+-rw-r--r--   0        0        0      137 2024-04-04 07:14:11.870328 charmcord-0.24.2/CharmCord/functions/Client/botID.py
+-rw-r--r--   0        0        0      149 2024-04-04 07:14:11.854368 charmcord-0.24.2/CharmCord/functions/Client/botMention.py
+-rw-r--r--   0        0        0      143 2024-04-04 07:14:11.902241 charmcord-0.24.2/CharmCord/functions/Client/botName.py
+-rw-r--r--   0        0        0      154 2024-04-04 07:14:11.877306 charmcord-0.24.2/CharmCord/functions/Client/ping.py
+-rw-r--r--   0        0        0     1223 2024-03-09 17:02:01.522527 charmcord-0.24.2/CharmCord/functions/clientActivity.py
+-rw-r--r--   0        0        0      403 2024-04-03 19:16:50.224079 charmcord-0.24.2/CharmCord/functions/Events/__init__.py
+-rw-r--r--   0        0        0     1367 2024-03-12 15:03:01.233500 charmcord-0.24.2/CharmCord/functions/Events/_options_.py
+-rw-r--r--   0        0        0      171 2024-04-03 19:17:35.455552 charmcord-0.24.2/CharmCord/functions/Events/deletedChannel.py
+-rw-r--r--   0        0        0      167 2024-04-03 19:17:35.451468 charmcord-0.24.2/CharmCord/functions/Events/memberJoined.py
+-rw-r--r--   0        0        0      163 2024-04-03 19:17:35.444186 charmcord-0.24.2/CharmCord/functions/Events/newChannel.py
+-rw-r--r--   0        0        0      163 2024-04-03 19:17:35.460722 charmcord-0.24.2/CharmCord/functions/Events/oldChannel.py
+-rw-r--r--   0        0        0      169 2024-04-03 19:16:50.198158 charmcord-0.24.2/CharmCord/functions/Events/reactionAdded.py
+-rw-r--r--   0        0        0      171 2024-04-03 19:16:50.208493 charmcord-0.24.2/CharmCord/functions/Events/reactionRemoved.py
+-rw-r--r--   0        0        0      403 2024-04-03 19:16:50.234419 charmcord-0.24.2/CharmCord/functions/Guilds/__init__.py
+-rw-r--r--   0        0        0      229 2024-03-09 17:02:01.497593 charmcord-0.24.2/CharmCord/functions/Guilds/guildID.py
+-rw-r--r--   0        0        0      450 2024-04-04 07:08:16.543821 charmcord-0.24.2/CharmCord/functions/Guilds/guildName.py
+-rw-r--r--   0        0        0      599 2024-04-04 07:10:02.301739 charmcord-0.24.2/CharmCord/functions/Guilds/guildTextChannels.py
+-rw-r--r--   0        0        0      403 2024-04-03 19:11:35.344498 charmcord-0.24.2/CharmCord/functions/Messages/__init__.py
+-rw-r--r--   0        0        0       25 2024-04-03 17:45:00.065444 charmcord-0.24.2/CharmCord/functions/Messages/_btnOpts_.py
+-rw-r--r--   0        0        0     2473 2024-04-04 06:49:04.962972 charmcord-0.24.2/CharmCord/functions/Messages/addButton.py
+-rw-r--r--   0        0        0      559 2024-04-03 19:16:50.250927 charmcord-0.24.2/CharmCord/functions/Messages/buttonSend.py
+-rw-r--r--   0        0        0      346 2024-03-09 17:02:01.499587 charmcord-0.24.2/CharmCord/functions/Messages/defer.py
+-rw-r--r--   0        0        0      455 2024-03-09 17:02:01.500584 charmcord-0.24.2/CharmCord/functions/Messages/deleteMessage.py
+-rw-r--r--   0        0        0      735 2024-03-09 17:02:01.500584 charmcord-0.24.2/CharmCord/functions/Messages/editMessage.py
+-rw-r--r--   0        0        0      300 2024-03-09 17:02:01.501582 charmcord-0.24.2/CharmCord/functions/Messages/mentions.py
+-rw-r--r--   0        0        0      394 2024-04-04 06:54:00.774631 charmcord-0.24.2/CharmCord/functions/Messages/message.py
+-rw-r--r--   0        0        0      388 2024-04-04 06:54:00.767650 charmcord-0.24.2/CharmCord/functions/Messages/messageAuthor.py
+-rw-r--r--   0        0        0      390 2024-04-04 06:54:00.781639 charmcord-0.24.2/CharmCord/functions/Messages/messageContent.py
+-rw-r--r--   0        0        0       67 2024-03-09 17:02:01.502579 charmcord-0.24.2/CharmCord/functions/Messages/messageID.py
+-rw-r--r--   0        0        0      392 2024-04-04 06:54:00.755682 charmcord-0.24.2/CharmCord/functions/Messages/messageMentions.py
+-rw-r--r--   0        0        0     1544 2024-04-04 00:08:30.208461 charmcord-0.24.2/CharmCord/functions/Messages/purge.py
+-rw-r--r--   0        0        0     2316 2024-04-04 00:07:36.109871 charmcord-0.24.2/CharmCord/functions/Messages/sendEmbed.py
+-rw-r--r--   0        0        0      997 2024-04-04 00:06:53.255340 charmcord-0.24.2/CharmCord/functions/Messages/sendMessage.py
+-rw-r--r--   0        0        0      469 2024-03-09 17:02:01.504574 charmcord-0.24.2/CharmCord/functions/Messages/slashSend.py
+-rw-r--r--   0        0        0     1424 2024-04-04 06:54:00.789640 charmcord-0.24.2/CharmCord/functions/Messages/waitMessage.py
+-rw-r--r--   0        0        0     1697 2024-03-09 17:02:01.505571 charmcord-0.24.2/CharmCord/functions/Messages/waitReaction.py
+-rw-r--r--   0        0        0      403 2024-04-03 19:16:50.229203 charmcord-0.24.2/CharmCord/functions/Python/__init__.py
+-rw-r--r--   0        0        0     1035 2024-03-09 17:02:01.508563 charmcord-0.24.2/CharmCord/functions/Python/charmAI.py
+-rw-r--r--   0        0        0       64 2024-03-09 17:02:01.508563 charmcord-0.24.2/CharmCord/functions/Python/console.py
+-rw-r--r--   0        0        0      278 2024-03-09 17:02:01.509560 charmcord-0.24.2/CharmCord/functions/Python/count.py
+-rw-r--r--   0        0        0      581 2024-03-11 09:10:42.723633 charmcord-0.24.2/CharmCord/functions/Python/divide.py
+-rw-r--r--   0        0        0      854 2024-03-09 17:02:01.506569 charmcord-0.24.2/CharmCord/functions/Python/ElIf.py
+-rw-r--r--   0        0        0      779 2024-03-09 17:02:01.509560 charmcord-0.24.2/CharmCord/functions/Python/getJson.py
+-rw-r--r--   0        0        0      852 2024-03-09 17:02:01.507566 charmcord-0.24.2/CharmCord/functions/Python/If.py
+-rw-r--r--   0        0        0      577 2024-03-11 05:59:49.520543 charmcord-0.24.2/CharmCord/functions/Python/multi.py
+-rw-r--r--   0        0        0     1955 2024-03-09 17:02:01.511594 charmcord-0.24.2/CharmCord/functions/Python/onlyIf.py
+-rw-r--r--   0        0        0       78 2024-03-10 20:37:06.628081 charmcord-0.24.2/CharmCord/functions/Python/pyEval.py
+-rw-r--r--   0        0        0      569 2024-03-11 09:10:42.717522 charmcord-0.24.2/CharmCord/functions/Python/sub.py
+-rw-r--r--   0        0        0      571 2024-03-09 17:02:01.512553 charmcord-0.24.2/CharmCord/functions/Python/sum.py
+-rw-r--r--   0        0        0      101 2024-03-09 17:02:01.512553 charmcord-0.24.2/CharmCord/functions/Python/wait.py
+-rw-r--r--   0        0        0      403 2024-04-03 19:16:50.187749 charmcord-0.24.2/CharmCord/functions/Users/__init__.py
+-rw-r--r--   0        0        0      182 2024-03-09 17:02:01.513550 charmcord-0.24.2/CharmCord/functions/Users/authorID.py
+-rw-r--r--   0        0        0      188 2024-03-09 17:02:01.514547 charmcord-0.24.2/CharmCord/functions/Users/authorName.py
+-rw-r--r--   0        0        0      355 2024-03-09 17:02:01.514547 charmcord-0.24.2/CharmCord/functions/Users/hasPerm.py
+-rw-r--r--   0        0        0      481 2024-04-04 07:04:39.105167 charmcord-0.24.2/CharmCord/functions/Users/sendDM.py
+-rw-r--r--   0        0        0      428 2024-04-04 07:08:16.560775 charmcord-0.24.2/CharmCord/functions/Users/userID.py
+-rw-r--r--   0        0        0      440 2024-04-04 07:08:16.572742 charmcord-0.24.2/CharmCord/functions/Users/userMention.py
+-rw-r--r--   0        0        0      434 2024-04-04 07:04:39.117135 charmcord-0.24.2/CharmCord/functions/Users/userName.py
+-rw-r--r--   0        0        0      403 2024-04-03 19:16:50.244746 charmcord-0.24.2/CharmCord/functions/Variables/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-04 06:58:15.526257 charmcord-0.24.2/CharmCord/functions/Variables/get.py
+-rw-r--r--   0        0        0      669 2024-04-04 07:00:42.664752 charmcord-0.24.2/CharmCord/functions/Variables/getServerVar.py
+-rw-r--r--   0        0        0      751 2024-04-04 07:00:42.654806 charmcord-0.24.2/CharmCord/functions/Variables/getUserVar.py
+-rw-r--r--   0        0        0      256 2024-03-09 17:02:01.519534 charmcord-0.24.2/CharmCord/functions/Variables/getVar.py
+-rw-r--r--   0        0        0      174 2024-03-09 17:02:01.519534 charmcord-0.24.2/CharmCord/functions/Variables/let.py
+-rw-r--r--   0        0        0      485 2024-03-09 17:02:01.520531 charmcord-0.24.2/CharmCord/functions/Variables/setServerVar.py
+-rw-r--r--   0        0        0      556 2024-03-09 17:02:01.520531 charmcord-0.24.2/CharmCord/functions/Variables/setUserVar.py
+-rw-r--r--   0        0        0      484 2024-03-09 17:02:01.521528 charmcord-0.24.2/CharmCord/functions/Variables/setVar.py
+-rw-r--r--   0        0        0      477 2024-04-03 17:49:57.082699 charmcord-0.24.2/CharmCord/globeHandler.py
+-rw-r--r--   0        0        0    13944 2024-04-04 07:22:05.334490 charmcord-0.24.2/CharmCord/tools.py
+-rw-r--r--   0        0        0       65 2024-03-09 17:02:01.526515 charmcord-0.24.2/CharmCord/utils/__init__.py
+-rw-r--r--   0        0        0     9945 2024-04-04 00:04:40.167585 charmcord-0.24.2/CharmCord/utils/CharmCord.py
+-rw-r--r--   0        0        0     2647 2024-04-04 08:18:21.572444 charmcord-0.24.2/CharmCord/utils/Cogs.py
+-rw-r--r--   0        0        0      352 2024-03-09 17:02:01.524520 charmcord-0.24.2/CharmCord/utils/CommandHandler.py
+-rw-r--r--   0        0        0     1001 2024-04-03 23:59:12.759697 charmcord-0.24.2/CharmCord/utils/Commands.py
+-rw-r--r--   0        0        0     2425 2024-04-04 08:18:21.588402 charmcord-0.24.2/CharmCord/utils/SlashCommands.py
+-rw-r--r--   0        0        0    35823 2024-03-09 17:02:01.528510 charmcord-0.24.2/LICENSE
+-rw-r--r--   0        0        0      914 2024-04-04 08:20:11.125313 charmcord-0.24.2/pyproject.toml
+-rw-r--r--   0        0        0     3219 2024-04-04 07:42:59.033234 charmcord-0.24.2/README.md
+-rw-r--r--   0        0        0     3809 1970-01-01 00:00:00.000000 charmcord-0.24.2/PKG-INFO
```

### Comparing `charmcord-0.24.1/CharmCord/all_functions.py` & `charmcord-0.24.2/CharmCord/all_functions.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/CharmErrorHandling.py` & `charmcord-0.24.2/CharmCord/CharmErrorHandling.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Channels/channelCategoryID.py` & `charmcord-0.24.2/CharmCord/functions/Channels/channelCategoryID.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Channels/channelCategoryName.py` & `charmcord-0.24.2/CharmCord/functions/Channels/channelCategoryName.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Channels/channelChangedRoles.py` & `charmcord-0.24.2/CharmCord/functions/Channels/channelChangedRoles.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Channels/channelCreated.py` & `charmcord-0.24.2/CharmCord/functions/Channels/channelCreated.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Channels/channelDelay.py` & `charmcord-0.24.2/CharmCord/functions/Channels/channelDelay.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Channels/channelMention.py` & `charmcord-0.24.2/CharmCord/functions/Channels/channelMention.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Channels/channelName.py` & `charmcord-0.24.2/CharmCord/functions/Channels/channelName.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Channels/channelNsfw.py` & `charmcord-0.24.2/CharmCord/functions/Channels/channelNsfw.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Channels/channelPosition.py` & `charmcord-0.24.2/CharmCord/functions/Channels/channelPosition.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Channels/channelType.py` & `charmcord-0.24.2/CharmCord/functions/Channels/channelType.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Channels/channelURL.py` & `charmcord-0.24.2/CharmCord/functions/Channels/channelURL.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/clientActivity.py` & `charmcord-0.24.2/CharmCord/functions/clientActivity.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Events/_options_.py` & `charmcord-0.24.2/CharmCord/functions/Events/_options_.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Guilds/guildTextChannels.py` & `charmcord-0.24.2/CharmCord/functions/Guilds/guildTextChannels.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Messages/addButton.py` & `charmcord-0.24.2/CharmCord/functions/Messages/addButton.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Messages/buttonSend.py` & `charmcord-0.24.2/CharmCord/functions/Messages/buttonSend.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Messages/editMessage.py` & `charmcord-0.24.2/CharmCord/functions/Messages/editMessage.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Messages/purge.py` & `charmcord-0.24.2/CharmCord/functions/Messages/purge.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Messages/sendEmbed.py` & `charmcord-0.24.2/CharmCord/functions/Messages/sendEmbed.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Messages/sendMessage.py` & `charmcord-0.24.2/CharmCord/functions/Messages/sendMessage.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Messages/waitMessage.py` & `charmcord-0.24.2/CharmCord/functions/Messages/waitMessage.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Messages/waitReaction.py` & `charmcord-0.24.2/CharmCord/functions/Messages/waitReaction.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Python/charmAI.py` & `charmcord-0.24.2/CharmCord/functions/Python/charmAI.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Python/divide.py` & `charmcord-0.24.2/CharmCord/functions/Python/divide.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Python/ElIf.py` & `charmcord-0.24.2/CharmCord/functions/Python/ElIf.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Python/getJson.py` & `charmcord-0.24.2/CharmCord/functions/Python/getJson.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Python/If.py` & `charmcord-0.24.2/CharmCord/functions/Python/If.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Python/multi.py` & `charmcord-0.24.2/CharmCord/functions/Python/multi.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Python/onlyIf.py` & `charmcord-0.24.2/CharmCord/functions/Python/onlyIf.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Python/sub.py` & `charmcord-0.24.2/CharmCord/functions/Python/sub.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Python/sum.py` & `charmcord-0.24.2/CharmCord/functions/Python/sum.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Variables/getServerVar.py` & `charmcord-0.24.2/CharmCord/functions/Variables/getServerVar.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Variables/getUserVar.py` & `charmcord-0.24.2/CharmCord/functions/Variables/getUserVar.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/functions/Variables/setUserVar.py` & `charmcord-0.24.2/CharmCord/functions/Variables/setUserVar.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/tools.py` & `charmcord-0.24.2/CharmCord/tools.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/utils/CharmCord.py` & `charmcord-0.24.2/CharmCord/utils/CharmCord.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/utils/Cogs.py` & `charmcord-0.24.2/CharmCord/utils/Cogs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from CharmCord.tools import checkArgCheck, checkArgs, findBracketPairs, noArguments, isValid
 from CharmCord.globeHandler import get_globals
 
 AC = {}
-class CharmCogs:
 
 
+class CharmCogs:
+
     @staticmethod
     def command_cogs(name, code):
         funcs = get_globals()[0]
         bots = get_globals()[1]
 
         @bots.command(name=name)
         async def go(ctx, *args, codes=code):
@@ -42,15 +43,17 @@
             func = f"""@bot.tree.command(name=name)
 async def go(ctx, {', '.join(new_args)}):
                             '''{description}
 
                             Args:
                                 {nl.join(arg_descripts)}
                             '''
+                            from CharmCord.globeHandler import get_globals
                             from CharmCord.tools import noArguments, slashArgs, findBracketPairs, lets
+                            funcs = get_globals()[0]
                             context = ctx
                             new = []
                             for i in arguments:
                                 new.append(eval(i['name']))
                             finalCode = await noArguments(codes, funcs, context)
                             finalCode = slashArgs(new, finalCode)
                             await findBracketPairs(finalCode, funcs, context)
```

### Comparing `charmcord-0.24.1/CharmCord/utils/Commands.py` & `charmcord-0.24.2/CharmCord/utils/Commands.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/CharmCord/utils/SlashCommands.py` & `charmcord-0.24.2/CharmCord/utils/SlashCommands.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from CharmCord.globeHandler import get_globals
-
-
 class SlashCommands:
 
     @staticmethod
     def slash_command(name, code, args: list[dict] = None, description=None, bot=None):
         types = {1: "str", 2: "int"}
         new_args = []
         arg_descripts = []
@@ -25,14 +22,15 @@
 @bot.tree.command(name=name)
 async def go(ctx, {', '.join(new_args)}):
                 '''{description}
                 
                 Args:
                     {nl.join(arg_descripts)}
                 '''
+                from CharmCord.globeHandler import get_globals
                 from CharmCord.tools import noArguments, slashArgs, findBracketPairs, lets
                 funcs = get_globals()[0]
                 context = ctx
                 new = []
                 for i in arguments:
                     new.append(eval(i['name']))
                 finalCode = await noArguments(codes, funcs, context)
@@ -42,14 +40,15 @@
                     lets.clear()
         """
         func2 = f"""
 @bot.tree.command(name=name)
 async def go(ctx, {', '.join(new_args)}):
                 '''{description}
                 '''
+                from CharmCord.globeHandler import get_globals
                 from CharmCord.tools import noArguments, slashArgs, findBracketPairs, lets
                 funcs = get_globals()[0]
                 context = ctx
                 new = []
                 finalCode = await noArguments(codes, funcs, context)
                 await findBracketPairs(finalCode, funcs, context)
                 if len(lets) >= 1:
```

### Comparing `charmcord-0.24.1/LICENSE` & `charmcord-0.24.2/LICENSE`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/pyproject.toml` & `charmcord-0.24.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "charmcord"
-version = "0.24.1"
+version = "0.24.2"
 description = "CharmCord is the best python string-based package for Discord bot devs"
 authors = ["Jade"]
 license = "MIT"
 readme = "README.md"
 classifiers= [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `charmcord-0.24.1/README.md` & `charmcord-0.24.2/README.md`

 * *Files identical despite different names*

### Comparing `charmcord-0.24.1/PKG-INFO` & `charmcord-0.24.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charmcord
-Version: 0.24.1
+Version: 0.24.2
 Summary: CharmCord is the best python string-based package for Discord bot devs
 License: MIT
 Author: Jade
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: charmcord Version: 0.24.1 Summary: CharmCord is the
+Metadata-Version: 2.1 Name: charmcord Version: 0.24.2 Summary: CharmCord is the
 best python string-based package for Discord bot devs License: MIT Author: Jade
 Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: discord-py
```

