Install ipfs

```
$ brew install ipfs
```

To initialize a node:

```
$ ipfs init
```

To run the node:

```
$ ipfs daemon
```

Copy files from one directory to another:

```
$ rsync -r src/ dist/
$ rsync -r build/contracts/ dist/
```

List peer nodes on ipfs:
```
$ ipfs swarm peers
```

Copy files to IPFS:
```
$ ipfs add -r dist/
> added QmTwJ7AhGtXYLEad6yeRTryFh7g3kBPx4vk5W6dVMefHmT dist/index.html
> added Qmf8cEYeGBvexUX3g4nFDWVACCccT8j3Tg7hSRJxJt1wKo dist
```

Now you can access the directory `dist/` using the hash.

Deploy (publish) the root folder on the IPFS so we can acces the distributed files with an url:
```
$ ipfs name publish Qmf8cEYeGBvexUX3g4nFDWVACCccT8j3Tg7hSRJxJt1wKo
> Published to QmUGkCNEyqM2Qcc6FPzJZ73KrtSqpmdqsepRv2PJbcFyGm: /ipfs/Qmf8cEYeGBvexUX3g4nFDWVACCccT8j3Tg7hSRJxJt1wKo
```

Browse to ` https://gateway.ipfs.io/ipfs/Qmf8cEYeGBvexUX3g4nFDWVACCccT8j3Tg7hSRJxJt1wKo `
And you're going to see the page appear and now you have a fully-decentralized application.

The app will stay online for 24h unless you pin it.
