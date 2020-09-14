# vcoinjs
Dead simple and easy to use JavaScript based Vcoin library. Inspired by [pybitcointools](https://github.com/vbuterin/pybitcointools)

# Getting started (Dev)
```bash
git clone https://github.com/lubhub612/vcoinjs.git
cd vcoinjs
yarn install
yarn build

# Dev flow
flow status
yarn build
yarn test
```

# Example usage
```javascript
var vcoinjs = require('vcoinjs')

var priv = vcoin.address.mkPrivKey(vccseed)

//var priv = bitcoinlovejs.address.mkPrivKey('witch collapse practice feed shame open despair creek road again ice least')
    
var privWIF = vcoinjs.address.privKeyToWIF(priv);
    
var pubKey = vcoinjs.address.privKeyToPubKey(priv,true);
    
const pubKeyHash =  vcoinjs.config.mainnet.pubKeyHash;
    
var tAddr = vcoinjs.address.pubKeyToAddr(pubKey,pubKeyHash);
    
console.log(privWIF);
   
console.log(pubKey);
    
console.log(priv);
   
console.log(tAddr);



```
