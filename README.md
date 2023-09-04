# blockchain-main

---

This is the hub of the blockchain project.

## Project Code

---

This project has three parts so far.  There is the API, the Admin Client, and the Mobile Client.  Eventually there will be a strategy to add a database, containerization, and more complex server configurations.  For now, the complete functionality can be tested with just these three applications.

### API
The API provides all of the services to the admin client and the mobile client.  It also manages the transaction pool, the creation of blocks, and the blockchain itself.

[Blockchain API](https://github.com/hunteryavitz/blockchain-api)

### Admin Client
The admin client serves as the merchant portal for both business and IT.  The admin can check transactions, transaction life cycles, inventory, etc.  They can also monitor under the hood, such as verifying blocks or the blockchain itself, taking readiness and liveness checks, and tracking network latency.  This makes the admin client a powerful, two-fold facing utility.

[Blockchain Admin Client](https://github.com/hunteryavitz/blockchain-client-admin)

### Mobile Client
The mobile client serves as the field user tool.  The user will submit transactions with various status types, such as `CREATED`, `SHIPPED`, `CANCELLED`.  These status types will map to the inventory and product fulfillment for a given distribution chain.  Once the user submits a transaction, the API adds this to the transaction pool which is staged to be added to the blockchain.

[Blockchain Mobile Client](https://github.com/hunteryavitz/blockchain-client-mobile)

## Project Resources

---

This is a repository of the resources this project involves.

### Wiki
The wiki is a resource repository for this project.  Anything miscellaneous is likely to be found here.

[Wiki](https://github.com/hunteryavitz/blockchain-main/wiki)

### Overview
This is a bird-eye view of the project as I intend it so far.  This is a living document, but will not likely be updated with any regularity.

[Overview](https://github.com/hunteryavitz/blockchain-main/wiki/Blockchain-Overview)

### Anatomy
This is a break down of the components of the blockchain, block, and transaction.  Many other features are disected here as well.

[Anatomy](https://github.com/hunteryavitz/blockchain-main/wiki/Blockchain-Anatomy)

## Background

---

Here is some background information about this project.  This will be updated as major work is completed.

### Version
v0.0.1 - Unreleased

### Last Updated
9/4/23

### Description
This project is a POC blockchain that validates transactions to establish a chain of custody for some entity type.

### Objective
This project marks an attempt to create a proof-of-concept blockchain network that can validate transactions to establish a chain of custody.  This service could be used with a CRUD application to monitor authenticity of transactions, such as **RECEIVED**, **DELIVERED**, etc.  An additional UI could be used to monitor the overall network state of the blockchain.

### Details
Details for this project are yet to come.  A brief desciption follows:

## Back-End

---

There will be a back-end service that accepts transaction requests and manage a queue.  It will distribute these transaction requests to a set of nodes.  These nodes will process the transactions by mining a crypto-block and assigning the tranactions to this.  Then the node will add the block to the blockchain and broadcast to the other nodes so they can also update their blockchains through a validation process.

## Front-End

---

### Admin Panel
There will be a front-end UI that will present to a blockchain network admin a series of dashboards and various levels of metrics to monitor the overall network health of the blockchain.  This could include **average rate of consensus**, **transaction backlog**, or **block-chain growth**.

### Merchant Portal
There will be a front-end UI that will present to a merchant a series of dashboards a various stages of transactions to monitor the overall throughput of transaction as they pertain to the merchant.  This could include **RECEIVED**, **SIGNED**, or **DELIVERED**.

### Mobile Client
There will be a front-end UI that will present to a field worker a client interface that can create, read, and update transactions.  Creating a transaction could represent an order creation.  Reading a transaction could be a simple list / detail interface.  Updating a transaction could represent changing status in the chain of custody, such as **RECEIVED**, **SIGNED**, or **DELIVERED**.

## Development

---

The following applications are needed for this project:

- [TBD]()

### Summary
The aim of this project is to build a blockchain network from scratch.  This is purely educational and **could not / should not** every be considered for a production environment.

### Extra
I'm attempting to journal the progress for future reference.  I'll be creating pages for each entry and marking them here.

- [7/9/23](https://github.com/hunteryavitz/blockchain-main/wiki/Blockchain-Journal-%E2%80%90-7-9-23)
- [8/27/23](https://github.com/hunteryavitz/blockchain-main/wiki/Blockchain-Journal-%E2%80%90-8-27-23)
- [9/3/](https://github.com/hunteryavitz/blockchain-main/wiki/Blockchain-Journal-%E2%80%90-9-3-23)
- [9/4/23](https://github.com/hunteryavitz/blockchain-main/wiki/Blockchain-Journal-%E2%80%90-9-4-23)

Feel free to download and enjoy without restrictions.

For questions or comments, please reach out to me at [h.yavitz@gmail.com](mailto:h.yavitz@gmail.com).
