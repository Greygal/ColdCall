ColdCall
========

A recruitment tool to scrape [zKillboard](https://zkillboard.com) using EVE Online pilot statistics.

ColdCall has been designed specifically for [Aideron Robotics](https://aideronrobotics.com) needs.  It has been shared here as a framework for forking new and exciting filters in the future.

Dependencies
------------
* [Python 2.7.x](http://www.python.org/getit/)
* [MySQLdb](http://mysql-python.sourceforge.net/MySQLdb.html#installation)
* Entity's [eveapi](https://github.com/ntt/eveapi) (Included as submodule)
* zkb.py (included until broken out... then submodule)
* mySQL instance
* [EVE Data Dump (SDE)](https://www.fuzzwork.co.uk/dump/) strongly recommended

How To Use ColdCall
-------------------
ColdCall is initially designed as a command-line script.  

1. Configure init.ini (or init_local.ini) with the required global variables.
  * **Don't forget User_agent!!**
2. Configure candidate_*.sql to suit your filtering needs
3. Run `coldcall.py [options]` from the command line
4. Wait... zKillboard API can take a while with big queries (~2500 kills/minute)
5. Enjoy reports (.csv)

Feel free to adjust main() to suit your queries.  Setup should be pretty flexible

License Info
------------
This tool is wholly reliant on [zKillboard](https://zkillboard.com).  As such, it serves to remind users of [zkb's T.O.S. agreement](https://zkillboard.com/information/tos/).  zKillboard is a resource created by players, for players.  ColdCall has been created to enable people to better utilize zKillboard data, specifically as a tool to track grouping trends.  

ColdCall is openly shared to comply with zKB's "...datamining, in an attempt to gain an unfair advantage over corporations and/or alliances, is not allowed" rules.  Always remember @wilw's rule: Don't be a dick.

###CCP Legal Stuff
EVE Online and the EVE logo are the registered trademarks of CCP hf. All rights are reserved worldwide. All other trademarks are the property of their respective owners. EVE Online, the EVE logo, EVE and all associated logos and designs are the intellectual property of CCP hf. All artwork, screenshots, characters, vehicles, storylines, world facts or other recognizable features of the intellectual property relating to these trademarks are likewise the intellectual property of CCP hf. CCP hf. has granted permission to EVSCO to use EVE Online and all associated logos and designs for promotional and information purposes on its website but does not endorse, and is not in any way affiliated with, EVSCO. CCP is in no way responsible for the content on or functioning of this website, nor can it be liable for any damage arising from the use of this website.
