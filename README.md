# battery-present

Check if a specific battery is present. Probably only works on Linux.

## Example

``` javascript
var batteryPresent = require('battery-present');

batteryPresent('BAT0', function(exists) {
  console.log(exists);
  // true
});
```

## Installation

``` bash
$ npm install battery-present
```

## API

``` javascript
var batteryPresent = require('battery-present');
```

### `batteryPresent([battery], callback)`

Given an optional _String_ `battery`, calls `callback(true)` if that `battery`
exists in the current system. Otherwise calls `callback(false)`.