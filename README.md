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

1. Configure init.ini (or init_local.ini) with the required global variables
2. Configure candidate_*.sql to suit your filtering needs
3. Run coldcall.py [options] from the command line
4. Wait... zKillboard API can take a while with big queries (~2500 kills/minute)
5. Enjoy reports (.csv)

Feel free to adjust main() to suit your queries.  Setup should be pretty flexible

