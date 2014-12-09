PlayerStat
==========

EECS 341 Databases final project

Prerequisites
-------------

 - Python3
 - [Tk GUI Toolkit](http://www.tkdocs.com/tutorial/install.html)
 - [Sqlite3](http://www.sqlite.org/docs.html)

Resources
---------

 - [Using Sqlite3 with Python3](http://zetcode.com/db/sqlite/datamanipulation/)

Running
-------

####Setup
```bash
virtualenv env
source env/bin/activate
pip install -r requirements.txt
```
[More info](http://docs.python-guide.org/en/latest/dev/virtualenvs/)

####Running
```bash
cd bin
./playerstat
```

####Cleanup
```bash
deactivate
```
Usage
-----

The application will spawn with two windows, one for inserting game data, and one for serching
players or teams.  When searching, the target is controlled by the 'Search Teams' checkbox.
The wildcard '%' is available for incomplete queries or broader searching.  
Double clicking on the player will display their per-game stats and clicking on a heading will 
sort by that stat, including name or game number.  In the insertion window, data can be inserted
into the database given that it satisfies all dependencies.  A stat can be left blank to insert 
a 0 into the table.