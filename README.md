<p align="center">
  <img src="https://github.com/BananoCoin/banano/blob/master/logo.png" width="50%" height="50%"/></p>


# What is Banano?
Banano is designed to be a feeless, instant, high throughput cryptocurrency for the meme economy. 

### Key features
* Banano utilizes a novel block-lettuce architecture.
* Instant and Feeless transactions.
* Fungible (& Edible).
* Daily potassium airdrops.
* Ripe for memes.
* Literally grows on trees, no mining required.
* Not a Shitcoin (until digested).
* No more confusing prefix, Bananos contain Banoshis.
* Replay Protection to stop attackers from executing replay attacks from chain X on chain Y and vice versa.

### Key facts
* Forked from NANO (raiblocks)
* Total Supply: 3,402,823,669.20
* Born in Feb. 2018, Mainnet launch April 1st, 2018

For more information, see [Banano.cc](https://banano.cc).

### Resources
- [Banano website](https://banano.cc)
- [Yellowpaper](https://banano.cc/)
- [Discord chat](https://chat.banano.cc)
- [Reddit](http://reddit.com/r/banano)
- [Fritter](http://twitter.com/bananocoin)
- [GitHub wiki](http://github.com/bananocoin/banano/wiki)
- [BananoVault](https://vault.banano.cc)
- [Telegram](https://t.me/joinchat/HX-rIQ-t9Ad2xRcJjztVzg)
- [Banano.how all links at a glance](http://banano.how/)

### Build instructions
- [Building Banano from source](https://github.com/BananoCoin/banano/wiki/Building-a-Bananode-from-sources)

### Building with CMake

When building Banano with CMake, you can configure which network to build for using the `ACTIVE_NETWORK` option:

```bash
cmake -DCMAKE_BUILD_TYPE=RelWithDebInfo \
      -DACTIVE_NETWORK=banano_live_network \
      -DNANO_TEST=ON .
```

**Valid `ACTIVE_NETWORK` values:**

| Network | Description |
|---------|-------------|
| `banano_dev_network` | Development network with low work parameters and publicly known genesis key |
| `banano_beta_network` | Beta network with normal work parameters and secret beta genesis key |
| `banano_live_network` | **Default.** Live production network with normal work parameters |
| `banano_test_network` | Test network with normal work parameters and secret test genesis key |

If you don't specify `ACTIVE_NETWORK`, it defaults to `banano_live_network`.

**Common build configurations:**

```bash
# Production build (default)
cmake -DCMAKE_BUILD_TYPE=Release .

# Development build with tests
cmake -DCMAKE_BUILD_TYPE=Debug \
      -DACTIVE_NETWORK=banano_dev_network \
      -DNANO_TEST=ON .

# Test network build
cmake -DCMAKE_BUILD_TYPE=RelWithDebInfo \
      -DACTIVE_NETWORK=banano_test_network \
      -DNANO_TEST=ON .
```

### Running a Docker node
- [Running a Docker node](https://github.com/BananoCoin/banano/wiki/Running-a-Docker-Bananode)

### Want to contribute?

### Contact us
You can reach us via the [Discord](https://chat.banano.cc) or our [Reddit](http://reddit.com/r/banano).
You can also [file an issue](http://github.com/bananocoin/banano/issues).

