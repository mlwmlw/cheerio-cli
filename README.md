cheerio-cli
===========
[![NPM Version][npm-image]][npm-url]

cheerio in command line

installation
-----------
    $ npm install cheerio-cli -g
    
Example 
-----------
    simple query 
    $ curl -s https://github.com/mlwmlw/cheerio-cli | cheerio -o text "span[itemprop=author]"
    mlwmlw

    first element
    $ curl -s https://github.com/mlwmlw/cheerio-cli/commits/master | cheerio "a.commit-tease-sha"
    07b0406

    output query elements size
    $ curl -s https://github.com/mlwmlw/cheerio-cli/commits/master | cheerio ".commit" -o size
    6

    query element attribute
    $ curl -s https://github.com/mlwmlw/cheerio-cli/commits/master | cheerio "meta[name=hostname]" -a content
    github.com	
 
    piping ouput
    $ curl -s https://github.com/mlwmlw/cheerio-cli | cheerio "#readme" | cheerio "h2" -o text
 
[npm-image]: https://img.shields.io/npm/v/cheerio-cli.svg?style=flat
[npm-url]: https://npmjs.org/package/cheerio-cli
