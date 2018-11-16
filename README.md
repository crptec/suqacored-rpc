suqacored-rpc
===============

A client library to connect to SUQA Core RPC in JavaScript.

## Get Started

suqacored-rpc for suqacore-node

```bash
git clone https://github.com/crptec/suqacored-rpc.git
cd suqacored-rpc
npm install suqacored-rpc
```

### Bitcore-node module
```
cd node_modules
rm -rf suqacored-rpc
ln -s ~/suqacored-rpc
```

## RpcClient

Config parameters : 

	- protocol : (string - optional) - (default: 'https') - Set the protocol to be used. Either `http` or `https`.
	- user : (string - optional) - (default: 'user') - Set the user credential.
	- pass : (string - optional) - (default: 'pass') - Set the password credential.
	- host : (string - optional) - (default: '127.0.0.1') - The host you want to connect with.
	- port : (integer - optional) - (default: 8332) - Set the port on which perform the RPC command.

## Examples

Config:
```javascript
var config = {
    protocol: 'http',
    user: 'suqa',
    pass: 'local321',
    host: '127.0.0.1',
    port: 18332
};
```
## Help 

You can dynamically access to the help of each method by doing
```
const RpcClient = require('suqacored-rpc');
var client = new RPCclient({
    protocol:'http',
    user: 'suqa',
    pass: 'local321', 
    host: '127.0.0.1', 
    port: 18332
});

```
## License

**Code released under [the MIT license](https://github.com/bitpay/bitcore/blob/master/LICENSE).**

Copyright 2013-2014 BitPay, Inc.
