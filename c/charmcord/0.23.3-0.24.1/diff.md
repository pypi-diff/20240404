# Comparing `tmp/charmcord-0.23.3.tar.gz` & `tmp/charmcord-0.24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charmcord-0.23.3.tar", max compression
+gzip compressed data, was "charmcord-0.24.1.tar", max compression
```

## Comparing `charmcord-0.23.3.tar` & `charmcord-0.24.1.tar`

### file list

```diff
@@ -1,96 +1,100 @@
--rw-r--r--   0        0        0      330 2024-03-09 17:02:01.479681 charmcord-0.23.3/CharmCord/__init__.py
--rw-r--r--   0        0        0     1700 2024-03-11 21:08:24.175130 charmcord-0.23.3/CharmCord/all_functions.py
--rw-r--r--   0        0        0      686 2024-03-09 17:02:01.479681 charmcord-0.23.3/CharmCord/CharmErrorHandling.py
--rw-r--r--   0        0        0      270 2024-03-09 17:02:01.521528 charmcord-0.23.3/CharmCord/functions/__init__.py
--rw-r--r--   0        0        0      202 2024-03-09 17:02:01.481635 charmcord-0.23.3/CharmCord/functions/Channels/__init__.py
--rw-r--r--   0        0        0      535 2024-03-09 17:02:01.482632 charmcord-0.23.3/CharmCord/functions/Channels/channelCategoryID.py
--rw-r--r--   0        0        0      648 2024-03-09 17:02:01.483630 charmcord-0.23.3/CharmCord/functions/Channels/channelCategoryName.py
--rw-r--r--   0        0        0      955 2024-03-09 17:02:01.483630 charmcord-0.23.3/CharmCord/functions/Channels/channelChangedRoles.py
--rw-r--r--   0        0        0     1190 2024-03-09 17:02:01.484627 charmcord-0.23.3/CharmCord/functions/Channels/channelCreated.py
--rw-r--r--   0        0        0      607 2024-03-09 17:02:01.484627 charmcord-0.23.3/CharmCord/functions/Channels/channelDelay.py
--rw-r--r--   0        0        0      156 2024-03-09 17:02:01.485625 charmcord-0.23.3/CharmCord/functions/Channels/channelID.py
--rw-r--r--   0        0        0      604 2024-03-09 17:02:01.486625 charmcord-0.23.3/CharmCord/functions/Channels/channelMention.py
--rw-r--r--   0        0        0      582 2024-03-09 17:02:01.486625 charmcord-0.23.3/CharmCord/functions/Channels/channelName.py
--rw-r--r--   0        0        0      620 2024-03-09 17:02:01.487620 charmcord-0.23.3/CharmCord/functions/Channels/channelNsfw.py
--rw-r--r--   0        0        0      608 2024-03-09 17:02:01.488625 charmcord-0.23.3/CharmCord/functions/Channels/channelPosition.py
--rw-r--r--   0        0        0      586 2024-03-09 17:02:01.488625 charmcord-0.23.3/CharmCord/functions/Channels/channelType.py
--rw-r--r--   0        0        0      574 2024-03-09 17:02:01.489615 charmcord-0.23.3/CharmCord/functions/Channels/channelURL.py
--rw-r--r--   0        0        0       15 2024-03-09 17:02:01.489615 charmcord-0.23.3/CharmCord/functions/Channels/threadAutoArchive.py
--rw-r--r--   0        0        0      202 2024-03-09 17:02:01.490612 charmcord-0.23.3/CharmCord/functions/Client/__init__.py
--rw-r--r--   0        0        0      120 2024-03-09 17:02:01.490612 charmcord-0.23.3/CharmCord/functions/Client/botAvatar.py
--rw-r--r--   0        0        0      111 2024-03-09 17:02:01.491609 charmcord-0.23.3/CharmCord/functions/Client/botGuilds.py
--rw-r--r--   0        0        0      108 2024-03-09 17:02:01.491609 charmcord-0.23.3/CharmCord/functions/Client/botID.py
--rw-r--r--   0        0        0      118 2024-03-09 17:02:01.492605 charmcord-0.23.3/CharmCord/functions/Client/botMention.py
--rw-r--r--   0        0        0      112 2024-03-09 17:02:01.492605 charmcord-0.23.3/CharmCord/functions/Client/botName.py
--rw-r--r--   0        0        0      123 2024-03-09 17:02:01.493603 charmcord-0.23.3/CharmCord/functions/Client/ping.py
--rw-r--r--   0        0        0     1223 2024-03-09 17:02:01.522527 charmcord-0.23.3/CharmCord/functions/clientActivity.py
--rw-r--r--   0        0        0      202 2024-03-09 17:02:01.493603 charmcord-0.23.3/CharmCord/functions/Events/__init__.py
--rw-r--r--   0        0        0      167 2024-03-09 17:02:01.494702 charmcord-0.23.3/CharmCord/functions/Events/deletedChannel.py
--rw-r--r--   0        0        0      163 2024-03-09 17:14:07.214354 charmcord-0.23.3/CharmCord/functions/Events/memberJoined.py
--rw-r--r--   0        0        0      159 2024-03-09 17:02:01.495599 charmcord-0.23.3/CharmCord/functions/Events/newChannel.py
--rw-r--r--   0        0        0      159 2024-03-09 17:02:01.496595 charmcord-0.23.3/CharmCord/functions/Events/oldChannel.py
--rw-r--r--   0        0        0     1367 2024-03-12 15:03:01.233500 charmcord-0.23.3/CharmCord/functions/Events/options.py
--rw-r--r--   0        0        0      165 2024-03-11 21:08:24.163162 charmcord-0.23.3/CharmCord/functions/Events/reactionAdded.py
--rw-r--r--   0        0        0      167 2024-03-11 21:08:24.169154 charmcord-0.23.3/CharmCord/functions/Events/reactionRemoved.py
--rw-r--r--   0        0        0      202 2024-03-09 17:02:01.497593 charmcord-0.23.3/CharmCord/functions/Guilds/__init__.py
--rw-r--r--   0        0        0      229 2024-03-09 17:02:01.497593 charmcord-0.23.3/CharmCord/functions/Guilds/guildID.py
--rw-r--r--   0        0        0      425 2024-03-09 17:02:01.498590 charmcord-0.23.3/CharmCord/functions/Guilds/guildName.py
--rw-r--r--   0        0        0      572 2024-03-09 17:02:01.498590 charmcord-0.23.3/CharmCord/functions/Guilds/guildTextChannels.py
--rw-r--r--   0        0        0      202 2024-03-09 17:02:01.499587 charmcord-0.23.3/CharmCord/functions/Messages/__init__.py
--rw-r--r--   0        0        0      346 2024-03-09 17:02:01.499587 charmcord-0.23.3/CharmCord/functions/Messages/defer.py
--rw-r--r--   0        0        0      455 2024-03-09 17:02:01.500584 charmcord-0.23.3/CharmCord/functions/Messages/deleteMessage.py
--rw-r--r--   0        0        0      735 2024-03-09 17:02:01.500584 charmcord-0.23.3/CharmCord/functions/Messages/editMessage.py
--rw-r--r--   0        0        0      300 2024-03-09 17:02:01.501582 charmcord-0.23.3/CharmCord/functions/Messages/mentions.py
--rw-r--r--   0        0        0      361 2024-03-09 17:02:01.501582 charmcord-0.23.3/CharmCord/functions/Messages/message.py
--rw-r--r--   0        0        0      357 2024-03-09 17:02:01.501582 charmcord-0.23.3/CharmCord/functions/Messages/messageAuthor.py
--rw-r--r--   0        0        0      359 2024-03-09 17:02:01.502579 charmcord-0.23.3/CharmCord/functions/Messages/messageContent.py
--rw-r--r--   0        0        0       67 2024-03-09 17:02:01.502579 charmcord-0.23.3/CharmCord/functions/Messages/messageID.py
--rw-r--r--   0        0        0      361 2024-03-09 17:02:01.503576 charmcord-0.23.3/CharmCord/functions/Messages/messageMentions.py
--rw-r--r--   0        0        0     1546 2024-03-09 17:02:01.503576 charmcord-0.23.3/CharmCord/functions/Messages/purge.py
--rw-r--r--   0        0        0     2291 2024-03-09 17:02:01.504574 charmcord-0.23.3/CharmCord/functions/Messages/sendEmbed.py
--rw-r--r--   0        0        0      594 2024-03-09 17:02:01.504574 charmcord-0.23.3/CharmCord/functions/Messages/sendMessage.py
--rw-r--r--   0        0        0      469 2024-03-09 17:02:01.504574 charmcord-0.23.3/CharmCord/functions/Messages/slashSend.py
--rw-r--r--   0        0        0     1397 2024-03-09 17:02:01.505571 charmcord-0.23.3/CharmCord/functions/Messages/waitMessage.py
--rw-r--r--   0        0        0     1697 2024-03-09 17:02:01.505571 charmcord-0.23.3/CharmCord/functions/Messages/waitReaction.py
--rw-r--r--   0        0        0      202 2024-03-09 17:02:01.507566 charmcord-0.23.3/CharmCord/functions/Python/__init__.py
--rw-r--r--   0        0        0     1035 2024-03-09 17:02:01.508563 charmcord-0.23.3/CharmCord/functions/Python/charmAI.py
--rw-r--r--   0        0        0       64 2024-03-09 17:02:01.508563 charmcord-0.23.3/CharmCord/functions/Python/console.py
--rw-r--r--   0        0        0      278 2024-03-09 17:02:01.509560 charmcord-0.23.3/CharmCord/functions/Python/count.py
--rw-r--r--   0        0        0      581 2024-03-11 09:10:42.723633 charmcord-0.23.3/CharmCord/functions/Python/divide.py
--rw-r--r--   0        0        0      854 2024-03-09 17:02:01.506569 charmcord-0.23.3/CharmCord/functions/Python/ElIf.py
--rw-r--r--   0        0        0      779 2024-03-09 17:02:01.509560 charmcord-0.23.3/CharmCord/functions/Python/getJson.py
--rw-r--r--   0        0        0      852 2024-03-09 17:02:01.507566 charmcord-0.23.3/CharmCord/functions/Python/If.py
--rw-r--r--   0        0        0      577 2024-03-11 05:59:49.520543 charmcord-0.23.3/CharmCord/functions/Python/multi.py
--rw-r--r--   0        0        0     1955 2024-03-09 17:02:01.511594 charmcord-0.23.3/CharmCord/functions/Python/onlyIf.py
--rw-r--r--   0        0        0       78 2024-03-10 20:37:06.628081 charmcord-0.23.3/CharmCord/functions/Python/pyEval.py
--rw-r--r--   0        0        0      569 2024-03-11 09:10:42.717522 charmcord-0.23.3/CharmCord/functions/Python/sub.py
--rw-r--r--   0        0        0      571 2024-03-09 17:02:01.512553 charmcord-0.23.3/CharmCord/functions/Python/sum.py
--rw-r--r--   0        0        0      101 2024-03-09 17:02:01.512553 charmcord-0.23.3/CharmCord/functions/Python/wait.py
--rw-r--r--   0        0        0      202 2024-03-09 17:02:01.513550 charmcord-0.23.3/CharmCord/functions/Users/__init__.py
--rw-r--r--   0        0        0      182 2024-03-09 17:02:01.513550 charmcord-0.23.3/CharmCord/functions/Users/authorID.py
--rw-r--r--   0        0        0      188 2024-03-09 17:02:01.514547 charmcord-0.23.3/CharmCord/functions/Users/authorName.py
--rw-r--r--   0        0        0      355 2024-03-09 17:02:01.514547 charmcord-0.23.3/CharmCord/functions/Users/hasPerm.py
--rw-r--r--   0        0        0      454 2024-03-09 17:02:01.514547 charmcord-0.23.3/CharmCord/functions/Users/sendDM.py
--rw-r--r--   0        0        0      401 2024-03-09 17:02:01.515544 charmcord-0.23.3/CharmCord/functions/Users/userID.py
--rw-r--r--   0        0        0      411 2024-03-09 17:02:01.515544 charmcord-0.23.3/CharmCord/functions/Users/userMention.py
--rw-r--r--   0        0        0      405 2024-03-09 17:02:01.516542 charmcord-0.23.3/CharmCord/functions/Users/userName.py
--rw-r--r--   0        0        0      202 2024-03-09 17:02:01.517539 charmcord-0.23.3/CharmCord/functions/Variables/__init__.py
--rw-r--r--   0        0        0       92 2024-03-09 17:02:01.517539 charmcord-0.23.3/CharmCord/functions/Variables/get.py
--rw-r--r--   0        0        0      640 2024-03-09 17:02:01.518538 charmcord-0.23.3/CharmCord/functions/Variables/getServerVar.py
--rw-r--r--   0        0        0      722 2024-03-09 17:02:01.518538 charmcord-0.23.3/CharmCord/functions/Variables/getUserVar.py
--rw-r--r--   0        0        0      256 2024-03-09 17:02:01.519534 charmcord-0.23.3/CharmCord/functions/Variables/getVar.py
--rw-r--r--   0        0        0      174 2024-03-09 17:02:01.519534 charmcord-0.23.3/CharmCord/functions/Variables/let.py
--rw-r--r--   0        0        0      485 2024-03-09 17:02:01.520531 charmcord-0.23.3/CharmCord/functions/Variables/setServerVar.py
--rw-r--r--   0        0        0      556 2024-03-09 17:02:01.520531 charmcord-0.23.3/CharmCord/functions/Variables/setUserVar.py
--rw-r--r--   0        0        0      484 2024-03-09 17:02:01.521528 charmcord-0.23.3/CharmCord/functions/Variables/setVar.py
--rw-r--r--   0        0        0    13770 2024-03-09 17:02:01.522527 charmcord-0.23.3/CharmCord/tools.py
--rw-r--r--   0        0        0       65 2024-03-09 17:02:01.526515 charmcord-0.23.3/CharmCord/utils/__init__.py
--rw-r--r--   0        0        0     9682 2024-03-12 15:06:56.304865 charmcord-0.23.3/CharmCord/utils/CharmCord.py
--rw-r--r--   0        0        0     2575 2024-03-13 06:11:26.199667 charmcord-0.23.3/CharmCord/utils/Cogs.py
--rw-r--r--   0        0        0      352 2024-03-09 17:02:01.524520 charmcord-0.23.3/CharmCord/utils/CommandHandler.py
--rw-r--r--   0        0        0     1029 2024-03-13 06:12:00.487551 charmcord-0.23.3/CharmCord/utils/Commands.py
--rw-r--r--   0        0        0     2365 2024-03-09 17:02:01.525517 charmcord-0.23.3/CharmCord/utils/SlashCommands.py
--rw-r--r--   0        0        0    35823 2024-03-09 17:02:01.528510 charmcord-0.23.3/LICENSE
--rw-r--r--   0        0        0      914 2024-03-13 06:22:13.437590 charmcord-0.23.3/pyproject.toml
--rw-r--r--   0        0        0     3226 2024-03-12 15:08:11.960313 charmcord-0.23.3/README.md
--rw-r--r--   0        0        0     3815 1970-01-01 00:00:00.000000 charmcord-0.23.3/PKG-INFO
+-rw-r--r--   0        0        0      333 2024-03-14 06:59:51.324104 charmcord-0.24.1/CharmCord/__init__.py
+-rw-r--r--   0        0        0     1739 2024-04-03 15:34:15.303034 charmcord-0.24.1/CharmCord/all_functions.py
+-rw-r--r--   0        0        0      686 2024-03-09 17:02:01.479681 charmcord-0.24.1/CharmCord/CharmErrorHandling.py
+-rw-r--r--   0        0        0      268 2024-04-04 00:06:53.266312 charmcord-0.24.1/CharmCord/functions/__init__.py
+-rw-r--r--   0        0        0      403 2024-04-03 19:16:50.219032 charmcord-0.24.1/CharmCord/functions/Channels/__init__.py
+-rw-r--r--   0        0        0      562 2024-04-04 07:14:11.909221 charmcord-0.24.1/CharmCord/functions/Channels/channelCategoryID.py
+-rw-r--r--   0        0        0      675 2024-04-04 07:14:11.829435 charmcord-0.24.1/CharmCord/functions/Channels/channelCategoryName.py
+-rw-r--r--   0        0        0      982 2024-04-04 07:14:11.842399 charmcord-0.24.1/CharmCord/functions/Channels/channelChangedRoles.py
+-rw-r--r--   0        0        0     1217 2024-04-04 07:14:11.930165 charmcord-0.24.1/CharmCord/functions/Channels/channelCreated.py
+-rw-r--r--   0        0        0      634 2024-04-04 07:14:11.914208 charmcord-0.24.1/CharmCord/functions/Channels/channelDelay.py
+-rw-r--r--   0        0        0      156 2024-03-09 17:02:01.485625 charmcord-0.24.1/CharmCord/functions/Channels/channelID.py
+-rw-r--r--   0        0        0      633 2024-04-04 07:14:11.861349 charmcord-0.24.1/CharmCord/functions/Channels/channelMention.py
+-rw-r--r--   0        0        0      609 2024-04-04 07:14:11.936150 charmcord-0.24.1/CharmCord/functions/Channels/channelName.py
+-rw-r--r--   0        0        0      647 2024-04-04 07:14:11.944127 charmcord-0.24.1/CharmCord/functions/Channels/channelNsfw.py
+-rw-r--r--   0        0        0      635 2024-04-04 07:14:11.883324 charmcord-0.24.1/CharmCord/functions/Channels/channelPosition.py
+-rw-r--r--   0        0        0      613 2024-04-04 07:14:11.888278 charmcord-0.24.1/CharmCord/functions/Channels/channelType.py
+-rw-r--r--   0        0        0      601 2024-04-04 07:14:11.895258 charmcord-0.24.1/CharmCord/functions/Channels/channelURL.py
+-rw-r--r--   0        0        0       51 2024-04-03 19:05:05.886849 charmcord-0.24.1/CharmCord/functions/Channels/threadAutoArchive.py
+-rw-r--r--   0        0        0      405 2024-04-03 19:16:50.193021 charmcord-0.24.1/CharmCord/functions/Client/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-04 07:14:11.848384 charmcord-0.24.1/CharmCord/functions/Client/botAvatar.py
+-rw-r--r--   0        0        0      142 2024-04-04 07:14:11.949114 charmcord-0.24.1/CharmCord/functions/Client/botGuilds.py
+-rw-r--r--   0        0        0      137 2024-04-04 07:14:11.870328 charmcord-0.24.1/CharmCord/functions/Client/botID.py
+-rw-r--r--   0        0        0      149 2024-04-04 07:14:11.854368 charmcord-0.24.1/CharmCord/functions/Client/botMention.py
+-rw-r--r--   0        0        0      143 2024-04-04 07:14:11.902241 charmcord-0.24.1/CharmCord/functions/Client/botName.py
+-rw-r--r--   0        0        0      154 2024-04-04 07:14:11.877306 charmcord-0.24.1/CharmCord/functions/Client/ping.py
+-rw-r--r--   0        0        0     1223 2024-03-09 17:02:01.522527 charmcord-0.24.1/CharmCord/functions/clientActivity.py
+-rw-r--r--   0        0        0      403 2024-04-03 19:16:50.224079 charmcord-0.24.1/CharmCord/functions/Events/__init__.py
+-rw-r--r--   0        0        0     1367 2024-03-12 15:03:01.233500 charmcord-0.24.1/CharmCord/functions/Events/_options_.py
+-rw-r--r--   0        0        0      171 2024-04-03 19:17:35.455552 charmcord-0.24.1/CharmCord/functions/Events/deletedChannel.py
+-rw-r--r--   0        0        0      167 2024-04-03 19:17:35.451468 charmcord-0.24.1/CharmCord/functions/Events/memberJoined.py
+-rw-r--r--   0        0        0      163 2024-04-03 19:17:35.444186 charmcord-0.24.1/CharmCord/functions/Events/newChannel.py
+-rw-r--r--   0        0        0      163 2024-04-03 19:17:35.460722 charmcord-0.24.1/CharmCord/functions/Events/oldChannel.py
+-rw-r--r--   0        0        0      169 2024-04-03 19:16:50.198158 charmcord-0.24.1/CharmCord/functions/Events/reactionAdded.py
+-rw-r--r--   0        0        0      171 2024-04-03 19:16:50.208493 charmcord-0.24.1/CharmCord/functions/Events/reactionRemoved.py
+-rw-r--r--   0        0        0      403 2024-04-03 19:16:50.234419 charmcord-0.24.1/CharmCord/functions/Guilds/__init__.py
+-rw-r--r--   0        0        0      229 2024-03-09 17:02:01.497593 charmcord-0.24.1/CharmCord/functions/Guilds/guildID.py
+-rw-r--r--   0        0        0      450 2024-04-04 07:08:16.543821 charmcord-0.24.1/CharmCord/functions/Guilds/guildName.py
+-rw-r--r--   0        0        0      599 2024-04-04 07:10:02.301739 charmcord-0.24.1/CharmCord/functions/Guilds/guildTextChannels.py
+-rw-r--r--   0        0        0      403 2024-04-03 19:11:35.344498 charmcord-0.24.1/CharmCord/functions/Messages/__init__.py
+-rw-r--r--   0        0        0       25 2024-04-03 17:45:00.065444 charmcord-0.24.1/CharmCord/functions/Messages/_btnOpts_.py
+-rw-r--r--   0        0        0     2473 2024-04-04 06:49:04.962972 charmcord-0.24.1/CharmCord/functions/Messages/addButton.py
+-rw-r--r--   0        0        0      559 2024-04-03 19:16:50.250927 charmcord-0.24.1/CharmCord/functions/Messages/buttonSend.py
+-rw-r--r--   0        0        0      346 2024-03-09 17:02:01.499587 charmcord-0.24.1/CharmCord/functions/Messages/defer.py
+-rw-r--r--   0        0        0      455 2024-03-09 17:02:01.500584 charmcord-0.24.1/CharmCord/functions/Messages/deleteMessage.py
+-rw-r--r--   0        0        0      735 2024-03-09 17:02:01.500584 charmcord-0.24.1/CharmCord/functions/Messages/editMessage.py
+-rw-r--r--   0        0        0      300 2024-03-09 17:02:01.501582 charmcord-0.24.1/CharmCord/functions/Messages/mentions.py
+-rw-r--r--   0        0        0      394 2024-04-04 06:54:00.774631 charmcord-0.24.1/CharmCord/functions/Messages/message.py
+-rw-r--r--   0        0        0      388 2024-04-04 06:54:00.767650 charmcord-0.24.1/CharmCord/functions/Messages/messageAuthor.py
+-rw-r--r--   0        0        0      390 2024-04-04 06:54:00.781639 charmcord-0.24.1/CharmCord/functions/Messages/messageContent.py
+-rw-r--r--   0        0        0       67 2024-03-09 17:02:01.502579 charmcord-0.24.1/CharmCord/functions/Messages/messageID.py
+-rw-r--r--   0        0        0      392 2024-04-04 06:54:00.755682 charmcord-0.24.1/CharmCord/functions/Messages/messageMentions.py
+-rw-r--r--   0        0        0     1544 2024-04-04 00:08:30.208461 charmcord-0.24.1/CharmCord/functions/Messages/purge.py
+-rw-r--r--   0        0        0     2316 2024-04-04 00:07:36.109871 charmcord-0.24.1/CharmCord/functions/Messages/sendEmbed.py
+-rw-r--r--   0        0        0      997 2024-04-04 00:06:53.255340 charmcord-0.24.1/CharmCord/functions/Messages/sendMessage.py
+-rw-r--r--   0        0        0      469 2024-03-09 17:02:01.504574 charmcord-0.24.1/CharmCord/functions/Messages/slashSend.py
+-rw-r--r--   0        0        0     1424 2024-04-04 06:54:00.789640 charmcord-0.24.1/CharmCord/functions/Messages/waitMessage.py
+-rw-r--r--   0        0        0     1697 2024-03-09 17:02:01.505571 charmcord-0.24.1/CharmCord/functions/Messages/waitReaction.py
+-rw-r--r--   0        0        0      403 2024-04-03 19:16:50.229203 charmcord-0.24.1/CharmCord/functions/Python/__init__.py
+-rw-r--r--   0        0        0     1035 2024-03-09 17:02:01.508563 charmcord-0.24.1/CharmCord/functions/Python/charmAI.py
+-rw-r--r--   0        0        0       64 2024-03-09 17:02:01.508563 charmcord-0.24.1/CharmCord/functions/Python/console.py
+-rw-r--r--   0        0        0      278 2024-03-09 17:02:01.509560 charmcord-0.24.1/CharmCord/functions/Python/count.py
+-rw-r--r--   0        0        0      581 2024-03-11 09:10:42.723633 charmcord-0.24.1/CharmCord/functions/Python/divide.py
+-rw-r--r--   0        0        0      854 2024-03-09 17:02:01.506569 charmcord-0.24.1/CharmCord/functions/Python/ElIf.py
+-rw-r--r--   0        0        0      779 2024-03-09 17:02:01.509560 charmcord-0.24.1/CharmCord/functions/Python/getJson.py
+-rw-r--r--   0        0        0      852 2024-03-09 17:02:01.507566 charmcord-0.24.1/CharmCord/functions/Python/If.py
+-rw-r--r--   0        0        0      577 2024-03-11 05:59:49.520543 charmcord-0.24.1/CharmCord/functions/Python/multi.py
+-rw-r--r--   0        0        0     1955 2024-03-09 17:02:01.511594 charmcord-0.24.1/CharmCord/functions/Python/onlyIf.py
+-rw-r--r--   0        0        0       78 2024-03-10 20:37:06.628081 charmcord-0.24.1/CharmCord/functions/Python/pyEval.py
+-rw-r--r--   0        0        0      569 2024-03-11 09:10:42.717522 charmcord-0.24.1/CharmCord/functions/Python/sub.py
+-rw-r--r--   0        0        0      571 2024-03-09 17:02:01.512553 charmcord-0.24.1/CharmCord/functions/Python/sum.py
+-rw-r--r--   0        0        0      101 2024-03-09 17:02:01.512553 charmcord-0.24.1/CharmCord/functions/Python/wait.py
+-rw-r--r--   0        0        0      403 2024-04-03 19:16:50.187749 charmcord-0.24.1/CharmCord/functions/Users/__init__.py
+-rw-r--r--   0        0        0      182 2024-03-09 17:02:01.513550 charmcord-0.24.1/CharmCord/functions/Users/authorID.py
+-rw-r--r--   0        0        0      188 2024-03-09 17:02:01.514547 charmcord-0.24.1/CharmCord/functions/Users/authorName.py
+-rw-r--r--   0        0        0      355 2024-03-09 17:02:01.514547 charmcord-0.24.1/CharmCord/functions/Users/hasPerm.py
+-rw-r--r--   0        0        0      481 2024-04-04 07:04:39.105167 charmcord-0.24.1/CharmCord/functions/Users/sendDM.py
+-rw-r--r--   0        0        0      428 2024-04-04 07:08:16.560775 charmcord-0.24.1/CharmCord/functions/Users/userID.py
+-rw-r--r--   0        0        0      440 2024-04-04 07:08:16.572742 charmcord-0.24.1/CharmCord/functions/Users/userMention.py
+-rw-r--r--   0        0        0      434 2024-04-04 07:04:39.117135 charmcord-0.24.1/CharmCord/functions/Users/userName.py
+-rw-r--r--   0        0        0      403 2024-04-03 19:16:50.244746 charmcord-0.24.1/CharmCord/functions/Variables/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-04 06:58:15.526257 charmcord-0.24.1/CharmCord/functions/Variables/get.py
+-rw-r--r--   0        0        0      669 2024-04-04 07:00:42.664752 charmcord-0.24.1/CharmCord/functions/Variables/getServerVar.py
+-rw-r--r--   0        0        0      751 2024-04-04 07:00:42.654806 charmcord-0.24.1/CharmCord/functions/Variables/getUserVar.py
+-rw-r--r--   0        0        0      256 2024-03-09 17:02:01.519534 charmcord-0.24.1/CharmCord/functions/Variables/getVar.py
+-rw-r--r--   0        0        0      174 2024-03-09 17:02:01.519534 charmcord-0.24.1/CharmCord/functions/Variables/let.py
+-rw-r--r--   0        0        0      485 2024-03-09 17:02:01.520531 charmcord-0.24.1/CharmCord/functions/Variables/setServerVar.py
+-rw-r--r--   0        0        0      556 2024-03-09 17:02:01.520531 charmcord-0.24.1/CharmCord/functions/Variables/setUserVar.py
+-rw-r--r--   0        0        0      484 2024-03-09 17:02:01.521528 charmcord-0.24.1/CharmCord/functions/Variables/setVar.py
+-rw-r--r--   0        0        0      477 2024-04-03 17:49:57.082699 charmcord-0.24.1/CharmCord/globeHandler.py
+-rw-r--r--   0        0        0    13944 2024-04-04 07:22:05.334490 charmcord-0.24.1/CharmCord/tools.py
+-rw-r--r--   0        0        0       65 2024-03-09 17:02:01.526515 charmcord-0.24.1/CharmCord/utils/__init__.py
+-rw-r--r--   0        0        0     9945 2024-04-04 00:04:40.167585 charmcord-0.24.1/CharmCord/utils/CharmCord.py
+-rw-r--r--   0        0        0     2515 2024-04-03 23:56:24.556283 charmcord-0.24.1/CharmCord/utils/Cogs.py
+-rw-r--r--   0        0        0      352 2024-03-09 17:02:01.524520 charmcord-0.24.1/CharmCord/utils/CommandHandler.py
+-rw-r--r--   0        0        0     1001 2024-04-03 23:59:12.759697 charmcord-0.24.1/CharmCord/utils/Commands.py
+-rw-r--r--   0        0        0     2349 2024-04-03 23:53:40.730100 charmcord-0.24.1/CharmCord/utils/SlashCommands.py
+-rw-r--r--   0        0        0    35823 2024-03-09 17:02:01.528510 charmcord-0.24.1/LICENSE
+-rw-r--r--   0        0        0      914 2024-04-04 07:43:18.730757 charmcord-0.24.1/pyproject.toml
+-rw-r--r--   0        0        0     3219 2024-04-04 07:42:59.033234 charmcord-0.24.1/README.md
+-rw-r--r--   0        0        0     3809 1970-01-01 00:00:00.000000 charmcord-0.24.1/PKG-INFO
```

### Comparing `charmcord-0.23.3/CharmCord/all_functions.py` & `charmcord-0.24.1/CharmCord/all_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 all_Funcs = [
     "$If",
     "$ElIf",
+    "$addButton",
+    "$buttonSend",
     "$authorID",
     "$botAvatar",
     "$botGuilds",
     "$botID",
     "$botMention",
     "$botName",
     "$channelCategoryID",
```

### Comparing `charmcord-0.23.3/CharmCord/CharmErrorHandling.py` & `charmcord-0.24.1/CharmCord/CharmErrorHandling.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.23.3/CharmCord/functions/Channels/channelCategoryID.py` & `charmcord-0.24.1/CharmCord/functions/Channels/channelURL.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from CharmCord.CharmErrorHandling import CharmCordErrors
+from CharmCord.globeHandler import get_globals
 
-
-async def channelCategoryID(args: str, context):
+async def channelURL(id, context):
     """
-    Ex. $channelCategoryID[ChannelID]
-    Returns the args of the current category args
+    Ex. $channelURL
+    returns the channel url to the given args
     """
-    from CharmCord.utils.CharmCord import bots
+    if len(id) < 1:
+        CharmCordErrors("No parameter provided for '$channelURL'")
+    bots = get_globals()[1]
 
     try:
-        channel = await bots.fetch_channel(args.replace("<#", "").replace(">", ""))
-        return channel.category.id
+        channel = await bots.fetch_channel(id.replace("<#", "").replace(">", ""))
+        return channel.jump_url
     except ValueError:
-        CharmCordErrors(f"$channelCategoryID: {args} not valid channel id\nCommand: {context.command.name}")
+        CharmCordErrors(f"$channelURL: {id} not valid channel id\nCommand: {context.command.name}")
```

### Comparing `charmcord-0.23.3/CharmCord/functions/Channels/channelCategoryName.py` & `charmcord-0.24.1/CharmCord/functions/Channels/channelCategoryName.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from CharmCord.CharmErrorHandling import CharmCordErrors
-
+from CharmCord.globeHandler import get_globals
 
 async def channelCategoryName(args, context):
     """
     Ex. $channelCategoryName[ChannelID]
     returns the name of the category name of the given args
     """
     if len(args) < 1:
         CharmCordErrors("No parameter provided for '$channelCategoryName'")
-    from CharmCord.utils.CharmCord import bots
+    bots = get_globals()[1]
 
     try:
         channel = await bots.fetch_channel(args.replace("<#", "").replace(">", ""))
         return channel.category.name
     except ValueError:
         CharmCordErrors(f"$channelCategoryName: {args} not valid channel id\nCommand: {context.command.name}")
```

### Comparing `charmcord-0.23.3/CharmCord/functions/Channels/channelChangedRoles.py` & `charmcord-0.24.1/CharmCord/functions/Channels/channelChangedRoles.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from CharmCord.CharmErrorHandling import CharmCordErrors
-
+from CharmCord.globeHandler import get_globals
 
 async def channelChangedRoles(args, context):
     """
     Ex. $channelChangedRoles[ChannelID;Index]
     """
     if len(args) < 1:
         CharmCordErrors("No parameter provided for '$channelChangedRoles'")
         return
-    from CharmCord.utils.CharmCord import bots
+    bots = get_globals()[1]
 
     if ";" in args:
         args = args.split(";")
         args = args[0]
         index = args[1]
         try:
             int(args)
```

### Comparing `charmcord-0.23.3/CharmCord/functions/Channels/channelCreated.py` & `charmcord-0.24.1/CharmCord/functions/Channels/channelCreated.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from CharmCord.CharmErrorHandling import CharmCordErrors
-
+from CharmCord.globeHandler import get_globals
 
 async def channelCreated(args: str, context, timezones, format_datetime):
     """
     Ex. $channelCreated[ChannelID]
     """
     if len(args) < 1:
         raise CharmCordErrors("No parameter provided for '$channelCreated'")
@@ -17,15 +17,15 @@
         try:
             ids, time = tuple(args.split(","))
             time = locals()[time.strip()]
         except:
             ids = args
             time = utc
 
-    from CharmCord.utils.CharmCord import bots
+    bots = get_globals()[1]
 
     try:
         channel = await bots.fetch_channel(ids.replace("<#", "").replace(">", ""))
 
         desiredDateForm = format_datetime(channel.created_at, form, time)
         if desiredDateForm != "ERROR":
             return desiredDateForm
```

### Comparing `charmcord-0.23.3/CharmCord/functions/Channels/channelDelay.py` & `charmcord-0.24.1/CharmCord/functions/Channels/channelType.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from CharmCord.CharmErrorHandling import CharmCordErrors
+from CharmCord.globeHandler import get_globals
 
-
-async def channelDelay(id, context):
+async def channelType(id, context):
     """
-    Ex. $channelDelay[ChannelID]
-    Returns the channel delay for the given channel args
+    Ex. $channelType[ChannelID]
+    returns the channel type of the given args
     """
     if len(id) < 1:
-        raise CharmCordErrors("No parameter provided for '$channelDelay'")
-    from CharmCord.utils.CharmCord import bots
+        CharmCordErrors("No parameter provided for '$channelType'")
+    bots = get_globals()[1]
 
     try:
         channel = await bots.fetch_channel(id.replace("<#", "").replace(">", ""))
-        return channel.delay
+        return channel.type
     except ValueError:
-        CharmCordErrors(f"$channelDelay: {id} not valid channel id\nCommand: {context.command.name}")
+        CharmCordErrors(f"$channelType: {id} not valid channel id\nCommand: {context.command.name}")
```

### Comparing `charmcord-0.23.3/CharmCord/functions/Channels/channelMention.py` & `charmcord-0.24.1/CharmCord/functions/Channels/channelMention.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from CharmCord.CharmErrorHandling import CharmCordErrors
+from CharmCord.globeHandler import get_globals
 
 
 async def channelMention(id, context):
     """
     Ex. $channelMention[ChannelID]
     returns a channel mention from the given args
     """
     if len(id) < 1:
         CharmCordErrors("No parameter provided for '$channelMention'")
-    from CharmCord.utils.CharmCord import bots
+    bots = get_globals()[1]
 
     try:
         channel = await bots.fetch_channel(id.replace("<#", "").replace(">", ""))
         return channel.mention
     except ValueError:
         CharmCordErrors(f"$channelMention: {id} not valid channel id\nCommand: {context.command.name}")
```

### Comparing `charmcord-0.23.3/CharmCord/functions/Channels/channelName.py` & `charmcord-0.24.1/CharmCord/functions/Channels/channelCategoryID.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from CharmCord.CharmErrorHandling import CharmCordErrors
+from CharmCord.globeHandler import get_globals
 
-
-async def channelName(id, context):
+async def channelCategoryID(args: str, context):
     """
-    Ex. $channelName[ChannelID]
-    returns channel name of the given args
+    Ex. $channelCategoryID[ChannelID]
+    Returns the args of the current category args
     """
-    if len(id) < 1:
-        CharmCordErrors("No parameter provided for '$channelName'")
-    from CharmCord.utils.CharmCord import bots
+    bots = get_globals()[1]
 
     try:
-        channel = await bots.fetch_channel(id.replace("<#", "").replace(">", ""))
-        return channel.name
+        channel = await bots.fetch_channel(args.replace("<#", "").replace(">", ""))
+        return channel.category.id
     except ValueError:
-        CharmCordErrors(f"$channelName: {id} not valid channel id\nCommand: {context.command.name}")
+        CharmCordErrors(f"$channelCategoryID: {args} not valid channel id\nCommand: {context.command.name}")
```

### Comparing `charmcord-0.23.3/CharmCord/functions/Channels/channelNsfw.py` & `charmcord-0.24.1/CharmCord/functions/Channels/channelNsfw.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from CharmCord.CharmErrorHandling import CharmCordErrors
-
+from CharmCord.globeHandler import get_globals
 
 async def channelNsfw(id, context):
     """
     Ex. $channelNsfw[ChannelID]
     returns a boolean about a channel nsfw setting
     """
     if len(id) < 1:
         CharmCordErrors("No parameter provided for '$channelNsfw'")
-    from CharmCord.utils.CharmCord import bots
+    bots = get_globals()[1]
 
     try:
         channel = await bots.fetch_channel(id.replace("<#", "").replace(">", ""))
         if channel.is_nsfw():
             return True
         else:
             return False
```

### Comparing `charmcord-0.23.3/CharmCord/functions/Channels/channelPosition.py` & `charmcord-0.24.1/CharmCord/functions/Channels/channelPosition.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from CharmCord.CharmErrorHandling import CharmCordErrors
-
+from CharmCord.globeHandler import get_globals
 
 async def channelPosition(id, context):
     """
     Ex. $channelPosition[ChannelID]
     returns the position of a given channel args
     """
     if len(id) < 1:
         CharmCordErrors("No parameter provided for '$channelPosition'")
-    from CharmCord.utils.CharmCord import bots
+    bots = get_globals()[1]
 
     try:
         channel = await bots.fetch_channel(id.replace("<#", "").replace(">", ""))
         return channel.position
     except ValueError:
         CharmCordErrors(f"$channelPosition: {id} not valid channel id\nCommand: {context.command.name}")
```

### Comparing `charmcord-0.23.3/CharmCord/functions/Channels/channelType.py` & `charmcord-0.24.1/CharmCord/functions/Channels/channelName.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from CharmCord.CharmErrorHandling import CharmCordErrors
+from CharmCord.globeHandler import get_globals
 
-
-async def channelType(id, context):
+async def channelName(id, context):
     """
-    Ex. $channelType[ChannelID]
-    returns the channel type of the given args
+    Ex. $channelName[ChannelID]
+    returns channel name of the given args
     """
     if len(id) < 1:
-        CharmCordErrors("No parameter provided for '$channelType'")
-    from CharmCord.utils.CharmCord import bots
+        CharmCordErrors("No parameter provided for '$channelName'")
+    bots = get_globals()[1]
 
     try:
         channel = await bots.fetch_channel(id.replace("<#", "").replace(">", ""))
-        return channel.type
+        return channel.name
     except ValueError:
-        CharmCordErrors(f"$channelType: {id} not valid channel id\nCommand: {context.command.name}")
+        CharmCordErrors(f"$channelName: {id} not valid channel id\nCommand: {context.command.name}")
```

### Comparing `charmcord-0.23.3/CharmCord/functions/clientActivity.py` & `charmcord-0.24.1/CharmCord/functions/clientActivity.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.23.3/CharmCord/functions/Events/options.py` & `charmcord-0.24.1/CharmCord/functions/Events/_options_.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.23.3/CharmCord/functions/Messages/editMessage.py` & `charmcord-0.24.1/CharmCord/functions/Messages/editMessage.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.23.3/CharmCord/functions/Messages/purge.py` & `charmcord-0.24.1/CharmCord/functions/Messages/purge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import discord
-
 from CharmCord.CharmErrorHandling import CharmCordErrors
 
 count = 0
 
 
 async def purge(args, context):
     global count
```

### Comparing `charmcord-0.23.3/CharmCord/functions/Messages/sendEmbed.py` & `charmcord-0.24.1/CharmCord/functions/Messages/sendEmbed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import discord
-
+from CharmCord.globeHandler import get_globals
 from CharmCord.all_functions import newline_char
 
 
 async def sendEmbed(args: str, context):
     """
     Ex. $sendEmbed[Channel args;Title;Message;Color?;image?;Footer?]
     Send an Embed
     """
-    from CharmCord.utils.CharmCord import bots
-
+    bots = get_globals()[1]
     args = args.replace(newline_char, "\n")
     split = args.split(";")
     try:
         channel_id = split[0]
         title = split[1]
         message = split[2]
         color = split[3]
```

### Comparing `charmcord-0.23.3/CharmCord/functions/Messages/sendMessage.py` & `charmcord-0.24.1/CharmCord/functions/Guilds/guildTextChannels.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from CharmCord.all_functions import newline_char
+import discord
+import CharmCord.CharmErrorHandling as ErrorHandling
+from CharmCord.globeHandler import get_globals
 
+EH = ErrorHandling.CharmErrorHandling()
 
-async def sendMessage(args: str, context):
-    from CharmCord.utils.CharmCord import bots
 
-    split = args.split(";")
-    if len(split) < 2:
-        raise SyntaxError("args or message not provided to $sendMessage")
+async def guildTextChannels(id, context):
+    bots = get_globals()[1]
+
     try:
-        channel_id = split[0]
-        message = split[1]
-        channel = await bots.fetch_channel(int(channel_id))
-        message = message.replace(newline_char, "\n")
-        sent = await channel.send(message)
-    except:
-        raise SyntaxError("Can't send empty message!")
-    return sent.id
+        id = int(id)
+        text = []
+        guild = await bots.fetch_guild(id)
+        channels = list(await guild.fetch_channels())
+        for channel in channels:
+            if isinstance(channel, discord.TextChannel):
+                text.append(channel.name)
+        return text
+    except ValueError:
+        EH.Errors(2, "None")
```

### Comparing `charmcord-0.23.3/CharmCord/functions/Messages/waitMessage.py` & `charmcord-0.24.1/CharmCord/functions/Messages/waitMessage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import asyncio
-
+from CharmCord.globeHandler import get_globals
 from CharmCord.CharmErrorHandling import CharmCordErrors
 
 
 async def waitMessage(args, context):
     """
     Ex. $waitMessage[ChannelID;User;timeout;timeoutErrMsg]
     """
-    from CharmCord.utils.CharmCord import bots
+    bots = get_globals()[1]
     split = args.split(";")
     if len(split) < 3:
         raise SyntaxError("args, User, or timeout not provided to $waitMessage")
     try:
         channel_id = split[0]
         user = split[1]
         timeout = int(split[2])
```

### Comparing `charmcord-0.23.3/CharmCord/functions/Messages/waitReaction.py` & `charmcord-0.24.1/CharmCord/functions/Messages/waitReaction.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.23.3/CharmCord/functions/Python/charmAI.py` & `charmcord-0.24.1/CharmCord/functions/Python/charmAI.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.23.3/CharmCord/functions/Python/divide.py` & `charmcord-0.24.1/CharmCord/functions/Python/divide.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.23.3/CharmCord/functions/Python/ElIf.py` & `charmcord-0.24.1/CharmCord/functions/Python/ElIf.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.23.3/CharmCord/functions/Python/getJson.py` & `charmcord-0.24.1/CharmCord/functions/Python/getJson.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.23.3/CharmCord/functions/Python/If.py` & `charmcord-0.24.1/CharmCord/functions/Python/If.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.23.3/CharmCord/functions/Python/multi.py` & `charmcord-0.24.1/CharmCord/functions/Python/multi.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.23.3/CharmCord/functions/Python/onlyIf.py` & `charmcord-0.24.1/CharmCord/functions/Python/onlyIf.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.23.3/CharmCord/functions/Python/sub.py` & `charmcord-0.24.1/CharmCord/functions/Python/sub.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.23.3/CharmCord/functions/Python/sum.py` & `charmcord-0.24.1/CharmCord/functions/Python/sum.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.23.3/CharmCord/functions/Variables/getUserVar.py` & `charmcord-0.24.1/CharmCord/functions/Variables/getUserVar.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
+from CharmCord.globeHandler import get_globals
 
 
 async def getUserVar(args, context):
-    from CharmCord.utils.CharmCord import all_vars
+    all_vars = get_globals()[2]
 
     ag = args.split(";")
     user = ag[0].replace("<@", "").replace(">", "")
     serverID = context.guild.id
     var = ag[1]
     try:
         with open("variables.json", "r") as variables:
```

### Comparing `charmcord-0.23.3/CharmCord/functions/Variables/setUserVar.py` & `charmcord-0.24.1/CharmCord/functions/Variables/setUserVar.py`

 * *Files identical despite different names*

### Comparing `charmcord-0.23.3/CharmCord/tools.py` & `charmcord-0.24.1/CharmCord/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 from datetime import datetime as d_t
 from pytz import timezone
-from CharmCord.all_functions import date_funcs, ifse
-from .functions import *
+from CharmCord.all_functions import date_funcs, ifse, all_Funcs, no_arg_Funcs
+from CharmCord.functions import *
 
 timezones = (timezone("EST"), timezone("UTC"), timezone("US/Pacific"))
 lets = {}
 
 
 class FunctionHandler:
     def __init__(self):
         self.funcs = {}
 
     def register_functions(self):
         for line in all_Funcs:
             function = eval(line.replace("$", ""))  # nosec
             self.funcs[line.replace("\n", "").lower()] = function
+            continue
 
     async def execute_functions(self, keyword, args, context):
         if keyword in ifse:
             check = await self.funcs[keyword](args, context)
             return check
         if keyword in date_funcs:
             return await self.funcs[keyword](args, context, timezones, format_datetime)
         return await self.funcs[keyword](args, context)
 
 
 async def noArguments(entry: str, functions, context):
-    from .all_functions import no_arg_Funcs
-
     for func in no_arg_Funcs:
         if func in entry:
             entry = entry.replace(
                 func,
                 str(await functions.execute_functions(func.lower(), None, context)),
             )
 
@@ -118,14 +117,16 @@
         test = [line.strip() for line in entry.split("\n") if len(line.strip()) >= 3]
     line = 0
     for code in new:
         line += 1
         if EndIf:
             if code.strip().startswith("$end"):
                 return
+            if code.strip().lower().startswith("$onlyif") and line != 1:
+                raise SyntaxError("$OnlyIf should only be at the beginning of a command")
             if code.strip().lower().startswith("$endif"):
                 continue
             elif code.strip().lower().startswith("$elif"):
                 if not any("$if" in Char.lower() for Char in test):
                     raise SyntaxError("No $If found in command before $ElIf")
                 EndIf = False
                 continue
```

### Comparing `charmcord-0.23.3/CharmCord/utils/CharmCord.py` & `charmcord-0.24.1/CharmCord/utils/CharmCord.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
 import discord
 from discord.ext import commands
-from CharmCord.functions.Events.options import options
+from CharmCord.functions.Events._options_ import options
+from CharmCord.functions.Messages._btnOpts_ import button
 from CharmCord.tools import FunctionHandler, findBracketPairs, noArguments
 from .CommandHandler import load_commands
 from .Commands import Commands
 from .SlashCommands import SlashCommands
+from ..globeHandler import update_globals, get_globals
 
-# Global Calls
-TotalFuncs = None
-bots = None
-all_vars = None
+global bots
 
 
 class CharmCord:
 
     def __init__(
             self,
             prefix,
@@ -77,14 +76,15 @@
                 command_prefix=self.prefix,
                 case_insensitive=self.case_insensitive,
                 intents=self.intent,
                 activity=self._activity,
                 help_command=self._help_command,
             )
         bots, self.bot = self._clients, self._clients
+        update_globals("bots", self.bot)
 
         try:
             load_commands(load_command_dir)
         except FileNotFoundError:
             pass
 
         try:
@@ -96,18 +96,23 @@
                 json.dump(go, var)
 
     @staticmethod
     def run(token: str):
         bots.run(token)
 
     def variables(self, variables: dict):
-        global all_vars
         for key, value in variables.items():
             self.all_variables[key] = value
         all_vars = self.all_variables
+        update_globals("all", all_vars)
+
+    @staticmethod
+    def button_code(name, code):
+        button[name] = code
+        return
 
     @staticmethod
     def slash_command(name: str, code: str, args: list[dict] = None, description: str = "") -> None:
         sl = SlashCommands().slash_command
         sl(name=name, code=code, args=args, description=description.lower(), bot=bots)
 
     @staticmethod
@@ -236,14 +241,15 @@
     # Global variables
     global bots
     global TotalFuncs
 
     # Initialize FunctionHandler and register functions
     functions = FunctionHandler()
     TotalFuncs = functions
+    update_globals("total", functions)
     functions.register_functions()
 
     # Create Start instance and return working bot
     _final = CharmCord(
         prefix,
         case_insensitive,
         intents,
```

### Comparing `charmcord-0.23.3/CharmCord/utils/Cogs.py` & `charmcord-0.24.1/CharmCord/utils/Cogs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-from CharmCord.utils.CharmCord import bots
 from CharmCord.tools import checkArgCheck, checkArgs, findBracketPairs, noArguments, isValid
+from CharmCord.globeHandler import get_globals
 
 AC = {}
-
-
 class CharmCogs:
 
+
     @staticmethod
     def command_cogs(name, code):
-        from .CharmCord import bots, TotalFuncs
+        funcs = get_globals()[0]
+        bots = get_globals()[1]
 
         @bots.command(name=name)
         async def go(ctx, *args, codes=code):
             context = ctx
             new_code = await checkArgCheck(args, codes, context)
             if new_code == "Failed":
                 return
-            code1 = await noArguments(new_code, TotalFuncs, context)
+            code1 = await noArguments(new_code, funcs, context)
             code2 = checkArgs(args, code1)
-            final_code = await isValid(code2, TotalFuncs)
-            await findBracketPairs(final_code, TotalFuncs, context)
+            final_code = await isValid(code2, funcs)
+            await findBracketPairs(final_code, funcs, context)
 
     @staticmethod
     def slashcommand_cogs(name, code, args: list[dict], description):
+
         def slash_command():
+            bots = get_globals()[1]
             types = {1: "str", 2: "int"}
             new_args = []
             arg_descripts = []
             for i in args:
                 if len(i) != 0:
                     try:
                         i['description']
                     except KeyError:
                         i['description'] = "No Description"
                     new_args.append(f"{i['name']}: {types[i['type']]}")
                     arg_descripts.append(f"{i['name']} ({types[i['type']]}): {i['description']}")
-            nl = "\n\t\t\t"
+            nl = "\n\t\t\t\t\t\t\t\t"
             needs = {"arguments": args, "codes": code, "bot": bots, "name": name}
-            func = f"""
-            @bot.tree.command(name=name)
-            async def go(ctx, {', '.join(new_args)}):
+            func = f"""@bot.tree.command(name=name)
+async def go(ctx, {', '.join(new_args)}):
                             '''{description}
 
                             Args:
                                 {nl.join(arg_descripts)}
                             '''
-                            from CharmCord.utils.CharmCord import TotalFuncs
                             from CharmCord.tools import noArguments, slashArgs, findBracketPairs, lets
                             context = ctx
                             new = []
                             for i in arguments:
                                 new.append(eval(i['name']))
-                            finalCode = await noArguments(codes, TotalFuncs, context)
+                            finalCode = await noArguments(codes, funcs, context)
                             finalCode = slashArgs(new, finalCode)
-                            await findBracketPairs(finalCode, TotalFuncs, context)
+                            await findBracketPairs(finalCode, funcs, context)
                             if len(lets) >= 1:
                                 lets.clear()
                     """
             exec(func, needs)
 
         slash_command()
```

### Comparing `charmcord-0.23.3/CharmCord/utils/Commands.py` & `charmcord-0.24.1/CharmCord/utils/Commands.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from CharmCord.tools import checkArgCheck, checkArgs, findBracketPairs, noArguments, lets, isValid
-
+from CharmCord.globeHandler import get_globals
 
 ########################################
 #              COMMANDS                #
 ########################################
 
 
 class Commands:
     # Global variables
 
     @staticmethod
     def command(name: str, code: str, aliases: list = [], bot=None):
-        from CharmCord.utils.CharmCord import TotalFuncs
         # Define command function dynamically
 
         @bot.command(name=name, aliases=aliases)
         async def go(ctx, *args, codes=code):
-            context = ctx
-            new_code = await checkArgCheck(args, codes, context)
+            funcs = get_globals()[0]
+            new_code = await checkArgCheck(args, codes, ctx)
             if new_code == "Failed":
                 return
-            code1 = await noArguments(new_code, TotalFuncs, context)
+            code1 = await noArguments(new_code, funcs, ctx)
             code2 = checkArgs(args, code1)
-            final_code = await isValid(code2, TotalFuncs)
-            await findBracketPairs(final_code, TotalFuncs, context)
+            final_code = await isValid(code2, funcs)
+            await findBracketPairs(final_code, funcs, ctx)
             if len(lets) >= 1:
                 lets.clear()
```

### Comparing `charmcord-0.23.3/CharmCord/utils/SlashCommands.py` & `charmcord-0.24.1/CharmCord/utils/SlashCommands.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from CharmCord.globeHandler import get_globals
+
+
 class SlashCommands:
 
     @staticmethod
     def slash_command(name, code, args: list[dict] = None, description=None, bot=None):
         types = {1: "str", 2: "int"}
         new_args = []
         arg_descripts = []
@@ -22,37 +25,37 @@
 @bot.tree.command(name=name)
 async def go(ctx, {', '.join(new_args)}):
                 '''{description}
                 
                 Args:
                     {nl.join(arg_descripts)}
                 '''
-                from CharmCord.utils.CharmCord import TotalFuncs
                 from CharmCord.tools import noArguments, slashArgs, findBracketPairs, lets
+                funcs = get_globals()[0]
                 context = ctx
                 new = []
                 for i in arguments:
                     new.append(eval(i['name']))
-                finalCode = await noArguments(codes, TotalFuncs, context)
+                finalCode = await noArguments(codes, funcs, context)
                 finalCode = slashArgs(new, finalCode)
-                await findBracketPairs(finalCode, TotalFuncs, context)
+                await findBracketPairs(finalCode, funcs, context)
                 if len(lets) >= 1:
                     lets.clear()
         """
         func2 = f"""
 @bot.tree.command(name=name)
 async def go(ctx, {', '.join(new_args)}):
                 '''{description}
                 '''
-                from CharmCord.utils.CharmCord import TotalFuncs
                 from CharmCord.tools import noArguments, slashArgs, findBracketPairs, lets
+                funcs = get_globals()[0]
                 context = ctx
                 new = []
-                finalCode = await noArguments(codes, TotalFuncs, context)
-                await findBracketPairs(finalCode, TotalFuncs, context)
+                finalCode = await noArguments(codes, funcs, context)
+                await findBracketPairs(finalCode, funcs, context)
                 if len(lets) >= 1:
                     lets.clear()
         """
         if args is None:
             exec(func2, needs)
         else:
             exec(func, needs)
```

### Comparing `charmcord-0.23.3/LICENSE` & `charmcord-0.24.1/LICENSE`

 * *Files identical despite different names*

### Comparing `charmcord-0.23.3/pyproject.toml` & `charmcord-0.24.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "charmcord"
-version = "0.23.3"
+version = "0.24.1"
 description = "CharmCord is the best python string-based package for Discord bot devs"
 authors = ["Jade"]
 license = "MIT"
 readme = "README.md"
 classifiers= [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `charmcord-0.23.3/README.md` & `charmcord-0.24.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,21 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/aoipy?color=green&label=downloads)
 ![Downloads](https://static.pepy.tech/personalized-badge/aoipy?period=total&units=international_system&left_color=grey&right_color=green&left_text=downloads)
 ![PyPI - License](https://img.shields.io/pypi/l/aoipy)
 ![](https://tokei.rs/b1/github/tomschimansky/aoipy)
 [![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
 
 ---
-![logo](https://github.com/LilbabxJJ-1/CharmCord/blob/master/CharmCord%20logo.png)
+![logo](https://github.com/LilbabxJJ-1/CharmCord/blob/master/CharmCord%20logo.png?raw=true)
 
 ---
-## v0.23.1
-
-- Added `$reactionAdd` and `$reactionRemove` events
-- Added new operation functions `$sub`, `$divide`, `$multi` 
+## v0.24.1
 
+- Added `$addButton` functions to be used
+- Rewrote a lot of codebase to conform to PEP8 Standards
 
 
 ## <span style="color:pink">CharmCord</span> Setups
 
 Install [CharmCord](https://pypi.org/charmcord)
 ```bash
 pip install CharmCord
```

#### html2text {}

```diff
@@ -3,36 +3,36 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/
 aoipy?color=green&label=downloads) ![Downloads](https://static.pepy.tech/
 personalized-badge/
 aoipy?period=total&units=international_system&left_color=grey&right_color=green&left_text=downloads)
 ![PyPI - License](https://img.shields.io/pypi/l/aoipy) ![](https://tokei.rs/b1/
 github/tomschimansky/aoipy) [![All Contributors](https://img.shields.io/badge/
 all_contributors-4-orange.svg?style=flat-square)](#contributors-) --- ![logo]
-(https://github.com/LilbabxJJ-1/CharmCord/blob/master/CharmCord%20logo.png) --
-- ## v0.23.1 - Added `$reactionAdd` and `$reactionRemove` events - Added new
-operation functions `$sub`, `$divide`, `$multi` ## CharmCord Setups Install
-[CharmCord](https://pypi.org/charmcord) ```bash pip install CharmCord ``` ####
-Warning: Package is still in beta, use at your own risk | feel free to report
-issues --- Simple Bot: ```python from CharmCord import CharmClient # ----------
------Imports-------------------- bot = CharmClient(prefix="!",
-case_insensitive=False, intents=("all",)) bot.variables({ "money": 199 })
-bot.on_ready( Code="$console[Bot is Ready]" ) bot.command( name="add-money",
-code=""" $setUserVar[$args[1];money;$args[2]] $sendMessage[$channelID;Added
-$$args[2] to $userName[$args[1]]'s account] """ # !add-money 123456789 300 #
-This would add money to the user variable then # send a confirmation message in
-the channel it # was invoked ) bot.command( name="Ping", # Command Name
-code=""" $sendMessage[$channelID; Pong!! $ping] """ # Command Code ) bot.run
-("*******<>***********") ``` --- Slash Interactions/Outside Commands/Activity:
-```python from CharmCord import CharmClient, setActivity # ---------------
-Imports-------------------- # Activity message is the actual status, the type
-is whether it'll # be a game status, listening status, etc act = setActivity
-(message="my servers", typing="watching") # For Commands outside the main.py
-file, you should add the # load_command_dir parameter with the name of your
-command file bot = CharmClient(prefix="!", case_insensitive=False, intents=
-("all",), activity=act, load_command_dir="Commands") bot.on_ready
-( code="$console[Bot is Ready]" ) bot.slash_command( name="repeat", # Name of
-the slash command args=["sentence"], # The required arguments
-description="Repeats what you say", # Description of command code="""
-$slashSend[$slashArgs[1]] """ # Code running on the command ) bot.run
-("*******<>***********") ``` ## New and still a work in progress ![](https://
-github.com/LilbabxJJ-1/CharmCord/blob/master/logo.gif) ## Contributors â¨
-_[_C_h_a_r_m_C_o_r_d_-_c_o_n_t_r_i_b_u_t_o_r_s_]
+(https://github.com/LilbabxJJ-1/CharmCord/blob/master/
+CharmCord%20logo.png?raw=true) --- ## v0.24.1 - Added `$addButton` functions to
+be used - Rewrote a lot of codebase to conform to PEP8 Standards ## CharmCord
+Setups Install [CharmCord](https://pypi.org/charmcord) ```bash pip install
+CharmCord ``` #### Warning: Package is still in beta, use at your own risk |
+feel free to report issues --- Simple Bot: ```python from CharmCord import
+CharmClient # ---------------Imports-------------------- bot = CharmClient
+(prefix="!", case_insensitive=False, intents=("all",)) bot.variables({ "money":
+199 }) bot.on_ready( Code="$console[Bot is Ready]" ) bot.command( name="add-
+money", code=""" $setUserVar[$args[1];money;$args[2]] $sendMessage
+[$channelID;Added $$args[2] to $userName[$args[1]]'s account] """ # !add-money
+123456789 300 # This would add money to the user variable then # send a
+confirmation message in the channel it # was invoked ) bot.command
+( name="Ping", # Command Name code=""" $sendMessage[$channelID; Pong!! $ping]
+""" # Command Code ) bot.run("*******<>***********") ``` --- Slash
+Interactions/Outside Commands/Activity: ```python from CharmCord import
+CharmClient, setActivity # ---------------Imports-------------------- #
+Activity message is the actual status, the type is whether it'll # be a game
+status, listening status, etc act = setActivity(message="my servers",
+typing="watching") # For Commands outside the main.py file, you should add the
+# load_command_dir parameter with the name of your command file bot =
+CharmClient(prefix="!", case_insensitive=False, intents=("all",), activity=act,
+load_command_dir="Commands") bot.on_ready( code="$console[Bot is Ready]" )
+bot.slash_command( name="repeat", # Name of the slash command args=
+["sentence"], # The required arguments description="Repeats what you say", #
+Description of command code=""" $slashSend[$slashArgs[1]] """ # Code running on
+the command ) bot.run("*******<>***********") ``` ## New and still a work in
+progress ![](https://github.com/LilbabxJJ-1/CharmCord/blob/master/logo.gif) ##
+Contributors â¨_[_C_h_a_r_m_C_o_r_d_-_c_o_n_t_r_i_b_u_t_o_r_s_]
```

### Comparing `charmcord-0.23.3/PKG-INFO` & `charmcord-0.24.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charmcord
-Version: 0.23.3
+Version: 0.24.1
 Summary: CharmCord is the best python string-based package for Discord bot devs
 License: MIT
 Author: Jade
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -27,22 +27,21 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/aoipy?color=green&label=downloads)
 ![Downloads](https://static.pepy.tech/personalized-badge/aoipy?period=total&units=international_system&left_color=grey&right_color=green&left_text=downloads)
 ![PyPI - License](https://img.shields.io/pypi/l/aoipy)
 ![](https://tokei.rs/b1/github/tomschimansky/aoipy)
 [![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
 
 ---
-![logo](https://github.com/LilbabxJJ-1/CharmCord/blob/master/CharmCord%20logo.png)
+![logo](https://github.com/LilbabxJJ-1/CharmCord/blob/master/CharmCord%20logo.png?raw=true)
 
 ---
-## v0.23.1
-
-- Added `$reactionAdd` and `$reactionRemove` events
-- Added new operation functions `$sub`, `$divide`, `$multi` 
+## v0.24.1
 
+- Added `$addButton` functions to be used
+- Rewrote a lot of codebase to conform to PEP8 Standards
 
 
 ## <span style="color:pink">CharmCord</span> Setups
 
 Install [CharmCord](https://pypi.org/charmcord)
 ```bash
 pip install CharmCord
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: charmcord Version: 0.23.3 Summary: CharmCord is the
+Metadata-Version: 2.1 Name: charmcord Version: 0.24.1 Summary: CharmCord is the
 best python string-based package for Discord bot devs License: MIT Author: Jade
 Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: discord-py
@@ -12,36 +12,36 @@
 charmcord) ![PyPI - Downloads](https://img.shields.io/pypi/dm/
 aoipy?color=green&label=downloads) ![Downloads](https://static.pepy.tech/
 personalized-badge/
 aoipy?period=total&units=international_system&left_color=grey&right_color=green&left_text=downloads)
 ![PyPI - License](https://img.shields.io/pypi/l/aoipy) ![](https://tokei.rs/b1/
 github/tomschimansky/aoipy) [![All Contributors](https://img.shields.io/badge/
 all_contributors-4-orange.svg?style=flat-square)](#contributors-) --- ![logo]
-(https://github.com/LilbabxJJ-1/CharmCord/blob/master/CharmCord%20logo.png) --
-- ## v0.23.1 - Added `$reactionAdd` and `$reactionRemove` events - Added new
-operation functions `$sub`, `$divide`, `$multi` ## CharmCord Setups Install
-[CharmCord](https://pypi.org/charmcord) ```bash pip install CharmCord ``` ####
-Warning: Package is still in beta, use at your own risk | feel free to report
-issues --- Simple Bot: ```python from CharmCord import CharmClient # ----------
------Imports-------------------- bot = CharmClient(prefix="!",
-case_insensitive=False, intents=("all",)) bot.variables({ "money": 199 })
-bot.on_ready( Code="$console[Bot is Ready]" ) bot.command( name="add-money",
-code=""" $setUserVar[$args[1];money;$args[2]] $sendMessage[$channelID;Added
-$$args[2] to $userName[$args[1]]'s account] """ # !add-money 123456789 300 #
-This would add money to the user variable then # send a confirmation message in
-the channel it # was invoked ) bot.command( name="Ping", # Command Name
-code=""" $sendMessage[$channelID; Pong!! $ping] """ # Command Code ) bot.run
-("*******<>***********") ``` --- Slash Interactions/Outside Commands/Activity:
-```python from CharmCord import CharmClient, setActivity # ---------------
-Imports-------------------- # Activity message is the actual status, the type
-is whether it'll # be a game status, listening status, etc act = setActivity
-(message="my servers", typing="watching") # For Commands outside the main.py
-file, you should add the # load_command_dir parameter with the name of your
-command file bot = CharmClient(prefix="!", case_insensitive=False, intents=
-("all",), activity=act, load_command_dir="Commands") bot.on_ready
-( code="$console[Bot is Ready]" ) bot.slash_command( name="repeat", # Name of
-the slash command args=["sentence"], # The required arguments
-description="Repeats what you say", # Description of command code="""
-$slashSend[$slashArgs[1]] """ # Code running on the command ) bot.run
-("*******<>***********") ``` ## New and still a work in progress ![](https://
-github.com/LilbabxJJ-1/CharmCord/blob/master/logo.gif) ## Contributors â¨
-_[_C_h_a_r_m_C_o_r_d_-_c_o_n_t_r_i_b_u_t_o_r_s_]
+(https://github.com/LilbabxJJ-1/CharmCord/blob/master/
+CharmCord%20logo.png?raw=true) --- ## v0.24.1 - Added `$addButton` functions to
+be used - Rewrote a lot of codebase to conform to PEP8 Standards ## CharmCord
+Setups Install [CharmCord](https://pypi.org/charmcord) ```bash pip install
+CharmCord ``` #### Warning: Package is still in beta, use at your own risk |
+feel free to report issues --- Simple Bot: ```python from CharmCord import
+CharmClient # ---------------Imports-------------------- bot = CharmClient
+(prefix="!", case_insensitive=False, intents=("all",)) bot.variables({ "money":
+199 }) bot.on_ready( Code="$console[Bot is Ready]" ) bot.command( name="add-
+money", code=""" $setUserVar[$args[1];money;$args[2]] $sendMessage
+[$channelID;Added $$args[2] to $userName[$args[1]]'s account] """ # !add-money
+123456789 300 # This would add money to the user variable then # send a
+confirmation message in the channel it # was invoked ) bot.command
+( name="Ping", # Command Name code=""" $sendMessage[$channelID; Pong!! $ping]
+""" # Command Code ) bot.run("*******<>***********") ``` --- Slash
+Interactions/Outside Commands/Activity: ```python from CharmCord import
+CharmClient, setActivity # ---------------Imports-------------------- #
+Activity message is the actual status, the type is whether it'll # be a game
+status, listening status, etc act = setActivity(message="my servers",
+typing="watching") # For Commands outside the main.py file, you should add the
+# load_command_dir parameter with the name of your command file bot =
+CharmClient(prefix="!", case_insensitive=False, intents=("all",), activity=act,
+load_command_dir="Commands") bot.on_ready( code="$console[Bot is Ready]" )
+bot.slash_command( name="repeat", # Name of the slash command args=
+["sentence"], # The required arguments description="Repeats what you say", #
+Description of command code=""" $slashSend[$slashArgs[1]] """ # Code running on
+the command ) bot.run("*******<>***********") ``` ## New and still a work in
+progress ![](https://github.com/LilbabxJJ-1/CharmCord/blob/master/logo.gif) ##
+Contributors â¨_[_C_h_a_r_m_C_o_r_d_-_c_o_n_t_r_i_b_u_t_o_r_s_]
```

