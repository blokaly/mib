## BIP39 and BIP44

```javascript
let aliceSeed = bip39.mnemonicToSeed('awesome bulb divert half alone dinner talk harbor swallow figure deliver scheme', '@LborHJH?NwI');
let alice = HDNode.fromSeedBuffer(aliceSeed, networks.testnet);
let child = alice.derivePath("m/44'/1'/0'/0/0");
console.log('alice btc address:', child.getAddress());
console.log('alice btc pub key:', child.keyPair.getPublicKeyBuffer().toString('hex'));
console.log('alice btc private key:', child.keyPair.toWIF());
```

```
alice btc address: n3A5DGn7AB8Y8rt5NBHBpNAm6RkWXeZ3eX
alice btc pub key: 03fd7a339cee75583375c284017ed0fe1fc806badd0505232eba12261b1fb1bc52
alice btc private key: cTD6ZsLnF1z2FREmkrSxKB3QaHLcsTqMoikxYM3sUZb2xpAGUUoU
```