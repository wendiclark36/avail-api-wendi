## Avail API Use Cases

Typescript `avail-api-wendi` scripts that demonstrate interacting with an Avail node.

Run an [Avail node on Spheron](https://docs.spheron.network/marketplace-guide/avail/)

### Install

Install:
```
    npm i
```

Install ts-node if needed
```
npm i -g avail-api-wendi
```

### Create Local Config 

Update: `config.ts` 

```typescript
export default {
    mnemonic: "", // The secret seed value for account used to sign transactions 
    ApiURL: "",   // Api url
    app_id: 0,    // Application id 
    amount: 0,    // Amount of tokens to transfer
    receiver: ""  // Receiver address
}
```

Connect to a node:
```
avail-api-wendi connect.ts 
```

Subscribes to new blocks:
```
avail-api-wendi listen_new_blocks.ts 
```