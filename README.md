cheerio-cli
===========

cheerio in command line

installation
-----------
    $ npm install cheerio-cli -g
    
example 
-----------
    $ curl -s https://github.com/mlwmlw/cheerio-cli | cheerio span[itemprop=title]
    mlwmlw
    $ curl -s https://github.com/mlwmlw/cheerio-cli/commits/master | cheerio .commit:last-child a:eq(1)
    07b0406
		$ curl -s https://github.com/mlwmlw/cheerio-cli/commits/master | cheerio .commit -o size
		6
