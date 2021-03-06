2048 solver bot
---------------

*This bot runs thru Selenium ChromeDriver and will connect directly to original web-version of 2048 game which host on http://gabrielecirulli.github.io/2048/ . This game will run all it JS's on client side so no need to worry about web-traffic or Gabriel's server loading.)*

###Dependencies

 - [Python 2.7](http://www.python.org) with [NumPy](http://www.numpy.org/) library
 - [Selenium bindings](https://pypi.python.org/pypi/selenium) for Python with [ChromeDriver](https://code.google.com/p/chromedriver/)

After installing ChromeDriver it needs to determine binaries location in script like this:

`chromedriver = "/Users/user/Downloads/chromedriver"`

###Usage
* **ResultLog.csv** -- log of all game played 
* **Batch-launcher.py** -- run 2048-solver-bot.py as multiple instances thru subprocess 
* **2048-solver-bot.py** -- the main script which solves

| **Arg** | **Full** | **Description** |
|-------|--------|---------------|  
|   -h | --help | Show help message and exit |  
|   -p | --play | Immediately starts playing after running |  
|   -a | --noanim | Remove tile animation to slightly sped up process |
| -g X | --games X | Play exact X games |
| -n STR | --note STR | Short note string <140 chrs in "quotes" will add to csv with each game result
| -d | --debug | Reserved for debugging purposes
| -l X | --loglevel X | Verbose level from 0 to 2 |