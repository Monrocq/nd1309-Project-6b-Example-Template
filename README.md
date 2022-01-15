# Supply chain & data auditing

This repository containts an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

---

##### Deploiment logs (contracts address) :

> Using network 'rinkeby'.

> Running migration: 1_initial_migration.js
> Replacing Migrations...
> ... 0x022b5de79395d340de3d9cca360c5b1096554923f0f083a4521b7d8a60603ae5
> Migrations: 0xed069be7deae5ff79597b15c3dd2cf9cf9f1e29b
> Saving successful migration to network...
> ... 0xb9abd2f9a912baf783d803e9b066eaa1fee3eab40492aeca887107dd4dd09f65
> Saving artifacts...
> Running migration: 2_deploy_contracts.js
> Replacing FarmerRole...
> ... 0xfe56c9512d18cb11685dcca6b36f27707a5e37e4b6ce46f1b7baf3ec91da04cd
> FarmerRole: 0x38fea39a12c9616090ea84b42636d8fab54403ea
> Replacing DistributorRole...
> ... 0x37d0996b09b93cf099c43985d647bcffd4b7bc8987b1d7cf22876bb824fa86a5
> DistributorRole: 0xc4c3631b001c04f511f8804d8936b35484485bbb
> Replacing RetailerRole...
> ... 0x910ae567a65a504bbe8e1c6b3f3d95c3ee40387c573e1c7922c716ac17b487f9
> RetailerRole: 0x59ec762103d2e916e4bac893d727b6b0cdc06767
> Replacing ConsumerRole...
> ... 0x610ac0d721f289e1251e2076681173aea9c807c03da3759ff1737d5db61ff1c8
> ConsumerRole: 0x9eba5fb4d6b441ff7cf1dc0c37a5155843f23d7b
> Replacing SupplyChain...
> ... 0xcdc02d941a57041388521754bf236039baf0c2fe24035c6aaa3c16cac0ad8c70
> SupplyChain: 0x34357512f33d572197ef4dfa14c0b1596932c772
> Saving successful migration to network...
> ... 0x856bb432d4a61648a4cbf4b7d0ea26c3061d901745a8b4618e950250d5e534d2
> Saving artifacts...

- Librairie used : `truffle-hdwallet-provider` --> Provide my wallet to deploy the smart contract
- Program version number :
  - Truffle v4.1.14 (core: 4.1.14)
  - Solidity v0.4.24 (solc-js)
- Node version : `v14.17.6`
- Web 3 version : `"web3": "^1.3.5"`

---

The DApp User Interface when running should look like...

![truffle test](images/ftc_product_overview.png)

![truffle test](images/ftc_farm_details.png)

![truffle test](images/ftc_product_details.png)

![truffle test](images/ftc_transaction_history.png)

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Please make sure you've already installed ganache-cli, Truffle and enabled MetaMask extension in your browser.

```
Give examples (to be clarified)
```

### Installing

> The starter code is written for **Solidity v0.4.24**. At the time of writing, the current Truffle v5 comes with Solidity v0.5 that requires function _mutability_ and _visibility_ to be specified (please refer to Solidity [documentation](https://docs.soliditylang.org/en/v0.5.0/050-breaking-changes.html) for more details). To use this starter code, please run `npm i -g truffle@4.1.14` to install Truffle v4 with Solidity v0.4.24.

A step by step series of examples that tell you have to get a development env running

Clone this repository:

```
git clone https://github.com/udacity/nd1309/tree/master/course-5/project-6
```

Change directory to `project-6` folder and install all requisite npm packages (as listed in `package.json`):

```
cd project-6
npm install
```

Launch Ganache:

```
ganache-cli -m "spirit supply whale amount human item harsh scare congress discover talent hamster"
```

Your terminal should look something like this:

![truffle test](images/ganache-cli.png)

In a separate terminal window, Compile smart contracts:

```
truffle compile
```

Your terminal should look something like this:

![truffle test](images/truffle_compile.png)

This will create the smart contract artifacts in folder `build\contracts`.

Migrate smart contracts to the locally running blockchain, ganache-cli:

```
truffle migrate
```

Your terminal should look something like this:

![truffle test](images/truffle_migrate.png)

Test smart contracts:

```
truffle test
```

All 10 tests should pass.

![truffle test](images/truffle_test.png)

In a separate terminal window, launch the DApp:

```
npm run dev
```

## Built With

- [Ethereum](https://www.ethereum.org/) - Ethereum is a decentralized platform that runs smart contracts
- [IPFS](https://ipfs.io/) - IPFS is the Distributed Web | A peer-to-peer hypermedia protocol
  to make the web faster, safer, and more open.
- [Truffle Framework](http://truffleframework.com/) - Truffle is the most popular development framework for Ethereum with a mission to make your life a whole lot easier.

## Authors

See also the list of [contributors](https://github.com/your/project/contributors.md) who participated in this project.

## Acknowledgments

- Solidity
- Ganache-cli
- Truffle
- IPFS
