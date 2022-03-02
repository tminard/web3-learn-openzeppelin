# OpenZeppelin Getting Started tutorial

From https://docs.openzeppelin.com/learn/.

# Running locally

Start the local blockchain network

```sh
$ npx ganache-cli --deterministic
```

Run tests

```sh
$ npx truffle test
```

Run the demo program

```sh
$ npx truffle exec --network development ./scripts/index.js
```

Migrate/deploy and launch interactive console

```sh
$ npx truffle migrate --network development
$ npx truffle console --network development
```

Now you can try a few things

```javascript
> const box = await Box.deployed();
> await box.store(42)
> await box.retrieve()
```