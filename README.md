# randomuser

[![CI](https://github.com/cascadiacollections/randomuser/actions/workflows/node.js.yml/badge.svg)](https://github.com/cascadiacollections/randomuser/actions/workflows/node.js.yml)
[![npm version](https://img.shields.io/npm/v/randomuser.svg?style=flat-square)](https://www.npmjs.com/package/randomuser)

## Installation

Install using the node.js package manager [npm](https://npmjs.org/):

    $ npm install randomuser

## Examples

Demos of the randomuser module are located in: [./examples](https://github.com/cascadiacollections/randomuser/tree/master/examples)

## Usage

### Require Module and Initialize Client

```javascript
var RandomUser = require('randomuser')
  , r = new RandomUser();
```

### .getUsers(callback)

```javascript
r.getUsers(function(data) {
  console.log(data);
});
```

### .getUsers(params, callback)

```javascript
r.getUsers({ seed: "foxie", results: 5, gender: "male" }, function(data) {
  console.log(data);
});
```

### params {Object} [Documentation](https://randomuser.me/)

* `results` - int specifying number of results to return
* `genders` - string - "male" or "female" specifying gender to generate
* `seed` - string - service will return same data for given seed

## Testing

    $ npm test

## Contributing

Feel free to contribute!
