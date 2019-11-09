# CSMM Economy Guide

One of the central functions of CSMM is the Economy system. When Economy is enabled, players have a virtual wallet that is available to them at all times, and can earn and spend money from that wallet in several different ways ways. This virtual wallet is completely separate from ingame Dukes.

Enabling the economy functionality is easy, but finding the right values to use for rewards and prices can be tricky. If you reward players too much, prices need to be extremely high to balance out, but if you set the rewards too low, players will be unable to use the custom commands and shop. There is no 'correct' values to use; how to reward, and how much, is unique to your server and how you administrators.

## Overview

### Earning Money
There are several unique ways to earn currency as a player, and the CSMM Server Admin can enable or disable each of these ways separately.

1. Playtime Rewards - Your server can be configured to reward people for being online. You choose how often the rewards go out, and how much players get as a reward. For example: every 15 minutes, all online players get 10 currency.
1. Kill Rewards - Players can receive currency rewards when they kill zombies, other players, or both. You choose how much each type of kill is worth.
1. Custom Commands/Hooks - When configuring Custom Commands or Custom Event Hooks, you can have the CSMM platform add currency to a player's balance. For example: a custom hook could detect when a player kills a Screamer, or a Rad Wight, and automatically give players a small currency bonus beyond the normal zombie kill reward.

### Spending Money
Once players have earned some currency, they can spend it several different ways, or even lose it, based on events that you configure.

1. Players can buy items from your Server Shop, if you have it configured.
1. If you have configured CSMM to connect to your Discord server, players can receive curreny for chatting on your server. You choose how often this reward can occur, and how much they get.
1. Both Built-in and Custon commands can be set to have a currency cost, preventing players from using it if they don't have enough cash.
1. Custom Event Hooks can be configured to remove currency from a player's wallet when they fire. For example: if a player kills another player, you can have CSMM reduce their wallet balance as a penalty.

## Configuring the Economy 

### Enabling the Economy module
The first step is to enable the Economy module in CSMM.

1. In the CSMM web UI, expand your server on the nav-panel to the left, and click Settings.
1. Inside Settings, find the 'Economy' pane and expand it.
1. At the top of the pane, you will see either a green or yellow button.
   1. If you see a green 'Enable Economy' button, click it to enable the Economy module.
   1. If you see a yellow 'Disable Economy' button, don't do anything, because the Economy module is already enabled.
   
### Configuring the Playtime Earner module
If you want to reward your players for being online and active, you can configure the Playtime Earner module.

1. In the Economy panel in CSMM Settings, click the Playtime Earner button.
1. Enable the module by clicking the checkbox at the top.
1. Set the Interval to the number of minutes that CSMM should wait before rewarding all online players with free currency.
1. Set the Rewart amount to a number that you wish players to receive periodically.
1. Click Save.

### Enabling the Kill Earner module
After the Playtime reward, next you should configure the Kill Earner feature.

1. In the Economy panel in CSMM Settings, click the Kill Earner button.
1. Enable the module by clicking the checkbox at the top.
1. Enter values for 'Player Kills' and 'Zombie Kills" to denote how much currency players will get when they kill other people, or mobs.

### Enabling the Discord Earner module [OPTIONAL]
Finally, for game servers with their own Discord server linked to CSMM, you can configure the optional Discord Text link capability.

1. In the Economy panel in CSMM Settings, click the Discord Text earner button.
1. Enable the module by clicking the checkbox at the top.
1. Configure how much currency a player gets for talking on Discord, and how often CSMM will wait before allowing them to earn currency again.
