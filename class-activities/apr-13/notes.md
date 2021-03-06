__MongoDB__
* noSQL database
* document oriented model not table relational model (sql)
* stores data in BSON format - compressed JSONs (binary structured object notation)
* tons of drivers and packages to connect to Node, C++, Java, etc

__relational databases__
* sql relies on Joins to comine relevent data
* wherea mongo is a document database, excels at heterogenous data formats

__storage__
* a database composed of multiple collection
    * a collection composed of multiple documents

__SQL terms compared to Mongo terms__
* in SQL --> in Mongo
    - database --> database
    - table --> collecion
    - row --> document
    - column --> field

__advantages of Mongo__
* able to add new fields
* able to do deep queries
* no migrations

__disadvantages of Mongo__
* less tools to analyze data (like workbench)

_if your database has a lot of relationships, it may make more sense to use sql, if not, Mongo may be beneficial_

__commands__
`mongod` - runs the database
`mongo` - the mongo shell, how we interact with our mongo database

`use lessondb` - creates lessondb and switches to it

`db` - tells which db you're currently using

`db.places.insert({"continent": "Africa", "country":"Morocco", "majorcities": ["Casablanca", "Fez", "Marrakech"]})` - creates a collection called places and gives it json document

- you can type .help() or .find() (i.e. db.places.help(), db.places.find())

__web scraping__
* pulling data out of another website
* we usually do this from an API, but when there is no API, scraping is a way to get it
* if terms of service from site, prohibit you from taking data from the site, then scraping would be a felony

__cheerio__
* extracts data from the DOM, _does not_ manipulate the DOM

__mongoose__
* can add behaviors
* you can 'populate' data to simulate a join
* use mongoose when you like working with bson data but you want more structure, more rules