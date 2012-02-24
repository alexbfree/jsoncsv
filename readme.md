
        __                                               
       |__|  ______ ____    ____    ____    _________  __
       |  | /  ___//  _ \  /    \ _/ ___\  /  ___/\  \/ /
       |  | \___ \(  <_> )|   |  \\  \___  \___ \  \   / 
    /\__|  |/____  >\____/ |___|  / \___  >/____  >  \_/  
    \______|     \/             \/      \/      \/        

    
---

# jsoncsv
- a json to csv library in javascript/coffeescript
  WIP.  this is specifically geared toward caremark data.
  am working on allowing any json format.

## Install

``` bash
npm install jsoncsv

```

## Usage Example in CoffeeScript

``` coffeescript
fs = require 'fs'
csvjs = require 'jsoncsv'

data = fs.readFileSync('data.json').toString()
jsoncsv.parse data, (err, row) -> 
  console.log row

```

## Usage Example in JavaScript

``` javascript
var jsoncsv, data, fs;
fs = require('fs');
jsoncsv = require('jsoncsv');

data = fs.readFileSync('data.json').toString();

jsoncsv.parse(data, function(err, row) {
  return console.log(row);
});

```

## Examples

* see example folder

## License

* see LICENSE

## Contributions

* Please submit any pull requests or issues.
