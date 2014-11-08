cheerio-cli
===========

cheerio in command line

installation
-----------
    $ npm install
    
example 
-----------
    $ curl -s https://github.com/mlwmlw/cheerio-cli | ./bin/cheerio span[itemprop=title]
    mlwmlw
    $ curl -s https://github.com/mlwmlw/cheerio-cli/commits/master | ./bin/cheerio .commit:last-child a:eq(1)
    07b0406
