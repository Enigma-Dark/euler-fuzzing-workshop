# Mastering Fuzzing

This repo contains all the details to follow along with the **Fuzzing Euler** workshop/talk. 


:star: The target audience includes both **smart contract developers** and **security people** looking to improve their testing practices and dive into the world of fuzzing.


:point_right: If you are already used to working with fuzzing the first part of this content may be a bit too basic for you :smiley:

# Suites
- [Ethereum vault kit](https://github.com/euler-xyz/euler-vault-kit)
- [EVC Playground](https://github.com/euler-xyz/evc-playground)
- [Reward Streams](https://github.com/euler-xyz/reward-streams.git)


## Workshop

First and foremost, clone any of the repositories above.

This project has been set up with a suite of tests that check for specific invariants for the reward streams, implemented by [vnmrtz.eth](https://twitter.com/vn_martinez_). These tests are located in the `test/invariants` directory. They are written in Solidity and are designed to be run with the [echidna](https://github.com/crytic/echidna) fuzzing tool.

Installation and usage of these tools is outside the scope of this README, but you can find more information in the respective repositories:
- [Echidna Installation](https://github.com/crytic/echidna)

To run invariant tests with Echidna:

```sh
./test/scripts/echidna.sh  
```

To run assert tests with Echidna:

```sh
./test/scripts/echidna-assert.sh  
```



