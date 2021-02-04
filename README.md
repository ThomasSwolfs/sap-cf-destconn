# sap-cf-destconn
NodeJS Library that wraps the calls for the destination and connectivity service

## Installation
using npm:

```bash
$ npm install -s sap-cf-destconn
```

## Example

### Read the destination configuration 

```js
    const {readDestination} = require('sap-cf-destconn');
    const destinationConfig = await readDestination("destinationName", "<JWT Token if you use Oauth2SAML or Oauth2USerToken>");
```

### Read the connectivity configuration 

```js
    const {readConnectivity} = require('sap-cf-destconn');
    const connectivityConfig = await readConnectivity("<locationID>", "<JWT Token if you use principal propagation>");
```
