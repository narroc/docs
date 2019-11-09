# CSMM Economy Guide

## Overview

One of the central functions of CSMM is the Economy system. When Economy is enabled, players have a virtual wallet that is available to them at all times, and can earn and spend money from that wallet in several different ways ways. This virtual wallet is completely separate from in-game Dukes, allowing you to have full control over how players receive this extra, external currency, as well as how and where and when they can spend it on.

From the earning side, players can receive currency for time played on the server, kills (both zombie and player), and via custom commands and events that can be configured in CSMM itself. Players can spend this currency at a configurable in-game/web-UI shop within CSMM, pay to use custom commands set up by the server Admins, and more.

Enabling the economy functionality is easy, but finding the right values to use for rewards and prices can be tricky. If you reward players too much, prices need to be extremely high to balance out, but if you set the rewards too low, players will be unable to use the custom commands and shop. There is no 'correct' values to use; how to reward, and how much, is unique to your server and how you administrators.

## Configuring the Economy 

### Enabling the Economy module
The first step is to enable the Economy module in CSMM.

1. In the CSMM web UI, expand your server on the nav-panel to the left, and click Settings.
1. Inside Settings, find the 'Economy' pane and expand it. Note that this is different from the Economy panel from the main server panel; that page hosts the server economy log files, not the configuration of the Economy itself.
1. At the top of the pane, you will see either a green or yellow button.
   1. If you see a green 'Enable Economy' button, click it to enable the Economy module.
   1. If you see a yellow 'Disable Economy' button, don't do anything, because the Economy module is already enabled.

### Set the currency name
Give your ingame currency a unique name so players can distinguish between it and other currencies, like Dukes.

1. In the Economy panel in CSMM Settings, click the Set Currency Name button.
1. In the Name field, set a simple name for the currency, like 'dollars' or 'zCoins' or something similar.
1. Click Save.

### Configuring the Playtime Earner module
Your server can be configured to reward people for being online. For example, your server could be configured so that every 15 minutes, all online players get 10 currency. The frequency of payments and the amount of currency the players get is configurable.

1. In the Economy panel in CSMM Settings, click the Playtime Earner button.
1. Enable the module by clicking the checkbox at the top.
1. Set the Interval to the number of minutes that CSMM should wait before rewarding all online players with free currency.
1. Set the Reward amount to a number that you wish players to receive periodically.
1. Click Save.

### Enabling the Kill Earner module
Players can receive currency rewards when they kill zombies, other players, or both. The reward for each type of kill can be configured separately.

1. In the Economy panel in CSMM Settings, click the Kill Earner button.
1. Enable the module by clicking the checkbox at the top.
1. Enter values for 'Player Kills' and 'Zombie Kills" to denote how much currency players will get when they kill other people, or mobs.

### Enabling the Discord Text Earner module
If your 7 Days server also has a Discord server for the community, you can link your Discord server with CSMM, and reward people for communicating on Discord by giving them currency when they chat. You can choose how much they get, and how often it will reward them for chatting. For example, you can set a currency reward of 10, and a timeout of 3600 seconds, meaning that once per hour, if they speak on Discord, they will earn 10 currency.

1. In the Economy panel in CSMM Settings, click the Discord Text earner button.
1. Enable the module by clicking the checkbox at the top.
1. Configure how much currency a player gets for talking on Discord, and how often CSMM will wait before allowing them to earn currency again.

## Spending Money
Once players have earned some currency, they can spend it several different ways, or even lose it, based on events that you configure.

1. Players can buy items from your Server Shop, if you have it configured. A guide is available for configuring the shop, and you can make as many or as few items available in the shop as you'd like.
1. Both Built-in and Custom commands can be set to have a currency cost, preventing players from using it if they don't have enough cash.
1. Custom Event Hooks can be configured to remove currency from a player's wallet when they trigger. For example: if a player kills another player, you can have CSMM reduce their wallet balance as a penalty.
