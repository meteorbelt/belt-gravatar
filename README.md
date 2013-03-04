# Meteor Belt Gravatar

Provides Gravatar API. For use with Meteor Belt applications

## Installation

Meteor Belt Gravatar can be installed with [Meteorite](https://github.com/oortcloud/meteorite/). From inside a Meteorite-managed app:

``` sh
$ mrt add belt-gravatar
```

## API

### Basics

```javascript
var params = {
  secure: true, // https ?
  d: encodeURIComponent('http://example.org'), // defalut
  s: 200, // size
  r: 'pg' // rating
};
var url = Belt.Gravatar.urlFromEmail('hello@meteorbelt.com', params);
test.equal(url, 'https://www.gravatar.com/avatar/44e00c6d4a1deab14c40c00c89844cac?d=http%3A%2F%2Fexample.org&s=200&r=pg');
```
