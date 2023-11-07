# Jazeker RP

Jazeker RP is a dutch fivem server. Here you'll find a great part of our resources, mlos, cars and eup. We intentionally choose to make our resources and additional content open source to improve the community and there content as a whole.

# The Silk Framework
Our server and framework in its roots is based uppon the qbcore framework and overextended framework. Because we use two diffrent frameworks we descided to agree uppon a couple of standards ourself, this way we can set a president to keep the development process easy for everyone who wants to contribute.

## Database
The database is one of the most crucial aspects for every fivem server because here you'll store the data of hunderst sometimes thousands of players. There for we decided that we need some standards for the table names, rows ids, etc.

### 1. Naming Conventions
The table names have the following format `<owner>_<feature>_<specification>`.

#### \<owner\>
The owner within the table name defines who owns and needs the data within the table and can therefor be one of the following things
- sv (short for server)
- pl (short for player)
- ch (short for character)

#### \<feature\>
The feature within the table name defines what feature the data is used for. For example your character has a phone so the table name becomes `char_phone` because it holds generic data for the phone of each character.

#### \<specification\>
The specification within the table name defines a specific part of a feature the data is used for. For example your character can send messages on the phone so the table name becomes `char_phone_messages` because it holds all the messages send on the phone by a character to another character. **It's important to know that this feature is not required this is only there to specify multibly dataset for a certain feature!**

### 2. Refrence Tables
The soul purpuse of refrence table is to join multible tables together that have no data in common, therefor a refrence table can only becreated for two owners in our case those refernce tables are `server_players` and `player_characters`.

## Resources
The resources are, next to a database, the things that give you're server that unique feel to it's mechanics and make people want to come back to it so they can play with there friends. Sinds by default the silk framework is made for roleplay but we are willing to support minigames in the future we need to set a president for the resources that we make to keep overview within the github org.

### 1. Naming Conventions
The resource names are a crucial aspect of a resource and therefor have the following format `slk-[<namespace>-]<gamemode>-<feature>-<specification>`

#### \[\<namespace\>\-]
Specifies the RAGE namespace it has the most (any%) of interaction with
- hud (`slk-hud-<feature>-<specification>`)
- vehicles (`slk-vehicle-<feature>-<specification>`)

#### [\<gamemode\>\-]
Like mentioned befor we want to support multiple gamemodes so we need to add the gamemode to also keep track of this. For the case that a resource can be used for multiple gamemodes we add the any gamemode
- any (Any Gamemode, `slk-any-<feature>-<specification>`)
- rp (Roleplay, `slk-rp-<feature>-<specification>`)

#### \<feature\>
A resource is always created for a feature therefor we need to add the feature to the resource name.
- `slk-rp-vehicles`
- `slk-rp-voip`
- `slk-rp-robberies`

#### \<specification\>
Sometimes a seperate resource is created for feature that allready exsist by will create a mess within the resource folder when a specification is added. Therefor we add a specification to a resource like shown below.
- `slk-rp-vehicle-keys`
- `slk-rp-vehicle-failure`
- `slk-rp-voip-radio`
- `slk-rp-voip-calls`
- `slk-rp-robbery-store`
- `slk-rp-robbery-bank`
