# Zombie Factory

The Zombie Factory is a Solidity project developed for personal practice. It allows users to create their own unique zombies through blockchain transactions. This project demonstrates the basics of smart contract development on the Ethereum blockchain, including creating and managing digital assets (zombies), generating random attributes, handling ownership, and event logging.

This project is inspired by and gives credit to [CryptoZombies.io](https://cryptozombies.io/), a free, interactive code school that teaches how to build games on Ethereum.

## Features

- **Create Zombie**: Users can create a new zombie by providing a name. The zombie's DNA is generated randomly.
- **Zombie Ownership**: Keeps track of which Ethereum address owns which zombie.
- **Event Logging**: Logs an event every time a new zombie is created.
- **Unique First Zombie**: Enforces that an address can only create a random zombie if they don't already own one.
- **CryptoKitties Integration**: Zombies can feed on CryptoKitties to mix their DNA.
- **Ownership and Control**: Ensures that zombies can only be fed by their owners.

## Contract Functions

### `ZombieFactory.sol`
- **`createRandomZombie`**: Create a zombie with a given name.

### `ZombieFeeding.sol`
- **`feedAndMultiply`**: Feed a zombie with the DNA of another creature and potentially create a new zombie with mixed DNA.
- **`feedOnKitty`**: Allows a zombie to feed on a specific CryptoKitty, affecting the zombie's DNA.

## Events

- **`NewZombie`**: Emitted when a new zombie is created, including its ID, name, and DNA.


