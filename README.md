# Police3
NPC Police replacement

# Upgrade
* At this time there may not be a direct upgrade path for settings. I will more than likely make a system to help migrate some player information, but due to the major changes I do not forsee a direct upgrade path at this time.
* For this reason, I will maintain the old police plugin for a couple major MC versions in the future.

# Major changes:   

## Guards
* Guards are no longer limited to NPC's (Though the plugin by default only has NPC guards and cameras [future]).
* Addons are able to implement their own guards if they want (players, etc..) via the API

## Wanted System
* Wanted status's are no longer a static setting. They are calculated on the fly based on location and bounty levels.
   * This will remove the ability to change a users status going forward. You can only change it by modifying the bounties.

## Bounties
* The bounty system supports Fines, or Time (seconds / set date).
   * Bounties can be marked as payable or not (Fines only, time has to be served)
* Bounties are now paied off per bounty. So as a player serves their times are able to be marked off with a bounty.
   * Bounties are served based on order of offense. Escapes are the last bounty to be served and are always marked as non-payable

## Jails
* You will no longer be required to have a jail on each world, or server (Bungeecord networks). You can have a single jail on a server/network now. Jails are found in order based on Town > World > Server > Network (Bungee)
  ** Bungeecord networks will have to assign the server to utilize if you have more than 1 jail on the network.

## Zones
* The plugin now supports zones. see [Zones](https://github.com/Nutty101/The_Fuzz/wiki/Zones) for more information.

## Worldguard Regions
* Regions are no longer able to flag a user with a wanted status. There may be an alternate to this, but at the time of this document the only planned items are security cameras
* WG regions in the end will only be utilized to link zones to a region (Shapes). This allows us to use a zone across multiple regions that are seperate and no need for setting the flags on each region. 

## Notoriety
* The Wanted level system has been correctly renamed to Notoriety.

## Security Cameras
* This may not make the initial release, but the system will implement cameras (Heads) that allow for camera guards (They cannot arrest players though, just monitoring)

## Ability to monitor assaults on more than NPCs
* Attack monitors many things now (Players, Villagers,[Passive Mobs](https://minecraft.gamepedia.com/Category:Passive_mobs) and [Neutral Mobs](https://minecraft.gamepedia.com/Category:Neutral_mobs), and NPCs)

