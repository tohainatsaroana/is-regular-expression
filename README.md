# ip-regex

> Regular expression for matching IP addresses
## Install

```sh
$ npm install is-regular-expression
```
## Usage

```js
import ipRegex from 'is-regular-expression';
// Contains an IP address?
ipRegex().test('unicorn 192.168.0.1');
//=> true
// Is an IP address?
ipRegex({exact: true}).test('unicorn 192.168.0.1');
//=> false
ipRegex.v6({exact: true}).test('1:2:3:4:5:6:7:8');
//=> true
```

## API

### ipRegex(options?)

Returns a regex for matching both IPv4 and IPv6.

### ipRegex.v4(options?)

Returns a regex for matching IPv4.

### ipRegex.v6(options?)

Returns a regex for matching IPv6.
