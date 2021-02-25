# Contracts ♚
This repository contains the contracts as they are deployed on the blockchain.

Contracts are flattned and contain all dependencies in one collective file.

## Updates
Gambit is a fork of Pancake's MasterChef contract, which is a fork of SushiSwap. To provide more
transparancy here is a list of patches made to the contract.

* Migrator Methods have been removed. These methods have been used in the past to perform rug pulls. We feel that keeping this code in place would not convey the trust we want our users to have
in the Gambit product.
* Double farming prevention. We adopted an addition to prevent mistakes in the addition of multiple farms for the same token.
* Timelock on all owner functions. No change can be made unless the change has been sumbitted to
a timelock contract that will inpose a manditory wait period of at lease 6 hours. This wait time will be increased over time.
* Deposit fees. There is a posibility added to charge a deposit fee on certain farms. This deposit fee is sent to a allocated public fee address, which can be used for buybacks and further development.
* Farming delegation. In some cases a farmed token can be delegated to another farming contract to
earn extra yield, which can be used to buy and burn Gambit tokens.
* Affiliate program

## Contract addresses

GambitKing: 0x92Ad1BB7A49C9c5eD253FdA37b63034F2eC0823A

GambitToken: 0x0d9699bF75752A4bf9754b7318c5c365da643f51

GambitPawn: 0x14bE6e45f27357A8f3F20a0517D90E7482eB4c1f

MultiCall: 0x6F291dA779f5fca42fC0d62451B5C60135E8ab12

Timelock: 0xF1e288fE5E386aA905F8A3e7aBFA0A41Eb9160c0
