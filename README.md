# csv-mongodb
[![Rate on Openbase](https://badges.openbase.io/js/rating/csv-mongodb.svg)](https://openbase.io/js/csv-mongodb?utm_source=embedded&utm_medium=badge&utm_campaign=rate-badge)

`csv-mongodb` module is a comprehensive nodejs package to handle csv upload  and to convert into your mongoDB database collection (with or without specifiying file path). It can be used as node.js library or in browser. Below are some features:
you
*  Work with millions of lines of data
*  Upload file Easily
*  Converts excel data to mongoDB database collection
*  Blazing fast
*  Give flexibility to developer with 'pre-defined' helpers



# csv-mongodb online 

[Here](http://dataeasy.herokuapp.com) is a free online excel/csv to mongodb convert service utilizing latest `csv-mongodb` module.

# Menu

* [Quick Start](#quick-start)
* [Contribution](#contribution)

# Quick Start

* [As Library](#library)

## Library

### Installation

```
npm i --save csv-mongodb
```

### From csv file to mongodb (Without path to file)

```js 
// No usage of multer and direct upload 

var csv=require('csv-mongodb')

// At post route of file upload 

app.post("/upload",csv.uploads('<name of input tag containing file'>),function(req,res){

csv.creation(req,<'url of your database connection'>,<'name of collection to be created'>)

})

```

### From csv file to mongodb (With path to file)

```js 
// Usage of multer  and multer storage 

var csv=require('csv-mongodb')

// At post route of file upload 

app.post("/upload",<'your multer middleware'>,function(req,res){

csv.creation(req,<'url of your database connection'>,<'name of collection to be created'>)

})

```



# Contribution

Very much appreciate any types of donation and support. 

## Code

`csv-mongodb` follows github convention for contributions. Here are some steps:

1. Fork the repo to your github account
2. Checkout code from your github repo to your local machine.
3. Make code changes and don't forget add related tests.
4. Run `npm test` locally before pushing code back.
5. Create a [Pull Request](https://help.github.com/articles/creating-a-pull-request/) on github.
6. Code review and merge
7. Changes will be published to NPM within next version.

