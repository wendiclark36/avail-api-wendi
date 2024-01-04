## Avail API Use Cases

Typescript `ts-node` scripts that demonstrate interacting with an Avail node.

Run an [Avail node on Spheron](https://docs.spheron.network/marketplace-guide/avail/)

### Install

Install:
```
    npm i
```

Install ts-node if needed
```
npm i -g ts-node
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
ts-node connect.ts 
```

Subscribes to new blocks:
```
ts-node listen_new_blocks.ts 
```