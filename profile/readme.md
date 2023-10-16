# Jazeker RP

Jazeker RP is a dutch fivem server. Here you'll find a great part of our resources, mlos, cars and eup. We intentionally choose to make our resources and additional content open source to improve the community and there content as a whole.

# The Silk Framework
Our server and framework in its roots is based uppon the qbcore framework and overextended framework. Because we use two diffrent frameworks we descided to agree uppon a couple of standards ourself, this way we can set a president to keep the development process easy for everyone who wants to contribute.

## Database
The database is most crucial aspects for every fivem server because here you'll store the data of hunderst sometimes thousands of players. There for we decided that we need some standards for the table names, rows ids, etc.

### 1. table names
The table names have the following format `<owner>_<feature>_<specification>`.

#### <owner>
The owner of within the table name difines who owns and needs the data within the table and can therefor be one of the following things
- sv (short for server)
- ply (short for player)
- char (short for character)

#### <feature>
The feature of within the table name difines what feature the data is used for. For example your character has a phone so the it becomes `char_phone`.

#### <specification>
The specification of within the table name difines a specific part of a feature the data is used for. For example your character can send messages on the phone so there for it becomes `char_phone_messages`. **It's important to know that this feature is not required this is only there to specify multibly dataset for a certain feature!**
