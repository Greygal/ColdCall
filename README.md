ColdCall
========

A recruitment tool to scrape [zKillboard](https://zkillboard.com) using EVE Online pilot statistics.

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
This tool is wholly reliant on [zKillboard](https://zkillboard.com).  As such, it serves to remind users of [zkb's T.O.S. agreement](https://zkillboard.com/information/tos/).  zKillboard is a resource created by players, for players.  ColdCall has been created for enabling people to better utilize zKillboard data in their recruiting process.  

ColdCall is openly shared to comply with zKB's "...datamining, in an attempt to gain an unfair advantage over corporations and/or alliances, is not allowed" rules.  Always remember @wilw's rule: Don't be a dick.
