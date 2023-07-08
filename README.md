# blockchain-main

This is the hub of the blockchain project.

[Blockchain API](https://github.com/hunteryavitz/blockchain-api)
[Blockchain Admin Client](https://github.com/hunteryavitz/blockchain-client-admin)
[Blockchain Mobile Client](https://github.com/hunteryavitz/blockchain-client-mobile)

---

**v0.0.1** - Unreleased

Last updated: 7/7/23

### Description
This project is a POC blockchain that validates transactions to establish a chain of custody for some entity type.

### Objective
This project marks an attempt to create a proof-of-concept blockchain network that can validate transactions to establish a chain of custody.  This service could be used with a CRUD application to monitor authenticity of transactions, such as **order received**, **order delivered**, etc.  An additional UI could be used to monitor the overall network state of the blockchain.

### Details
Details for this project are yet to come.  A brief desciption follows:

### [Back-End]()

There will be a back-end service that accepts transaction requests and manage a queue.  It will distribute these transaction requests to a set of nodes.  These nodes will process the transactions by mining a crypto-block and assigning the tranactions to this.  Then the node will add the block to the blockchain and broadcast to the other nodes so they can also update their blockchains through a validation process.

### [Front-End]()

**Admin Panel**

There will be a front-end UI that will present to a blockchain network admin a series of dashboards and various levels of metrics to monitor the overall network health of the blockchain.  This could include **average rate of consensus**, **transaction backlog**, or **block-chain growth**.

**Merchant Portal**

There will be a front-end UI that will present to a merchant a series of dashboards a various stages of transactions to monitor the overall throughput of transaction as they pertain to the merchant.  This could include **order received**, **order signed by**, or **order delivered**.

**[Mobile Client]()**

There will be a front-end UI that will present to a field worker a client interface that can create, read, and update transactions.  Creating a transaction could represent an order creation.  Reading a transaction could be a simple list / detail interface.  Updating a transaction could represent changing status in the chain of custody, such as **received**, **signed for**, or **delivered**.

### Development

The following applications are needed for this project:

- [TBD]()

### Summary
The aim of this project is to build a blockchain network from scratch.  This is purely educational and **could not / should not** every be considered for a production environment.

### Extra

[Project Anatomy]()

[Project Overview]()

Feel free to download and enjoy without restrictions.

For questions or comments, please reach out to me at [h.yavitz@gmail.com](mailto:h.yavitz@gmail.com).
