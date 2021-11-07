# Welcome to KarmaNet

Hello colleagues, I hope you are all well. As you all may know i just recently joined Zbank and I am very excited to be working with all of you. I have been asked to set up a private testnet for us to explore potentials for blockchain at Zbank for my first project. Given that this is a testnet, you are all free to experiment with the environment. 

![Bank](https://m.bankingexchange.com/media/k2/items/cache/9319bba24c84d8d9edf402bf20ff8909_XL.jpg?t=20170822_205447)

### **Instructions for setup and use:**

The name of the block chain network is Karmanet, to use the network you will need to run puppeth then name the network. You will need to manage the existing genesis and export the genesis configurations to a folder on your device so you can access the karmanet.json file.

In order to access the two nodes in the blockchain you will need to run the geth initialize command line in your git bash terminal. 

Initialize nodes: 
- ./geth --datadir node1 init karmanet.json
- ./geth --datadir node2 init karmanet.json

After initializing both nodes you will need to run code each node in a seperate terminal unlock each node to prepare it for mining by running the following code.

Set up nodes for mining:
- ./geth --datadir node1 --unlock "0x6Dd95f58819c72FB5e93712997Aa12Dbb4c9FEEB" --mine --rpc --allow-insecure-unlock
- ./geth --datadir node2 --unlock "0xAFD42957b680BfF188D98CE8d40BA794AbBf946A" --mine --port 30304 --bootnodes "enode://ac95810828228259627098da243875478144658d15025f6f18739ef81b6b0b2889d2cb0c2df15d6abe001165e6df2dc556eac572ff437eea17479fc653719b48@100.11.141.79:30303" --ipcdisable --allow-insecure-unlock

The password for the first node is "access" while the password for the second node is "access2". You will need these two passwords in order to be able to begin mining blocks.

### Blockchain access and key configurations:

**Network name:** karmanet

**Chain/network ID:** 41318

**Blocktime:** 15

**Node 1**
- Password: access
- Public address: 0x6Dd95f58819c72FB5e93712997Aa12Dbb4c9FEEB
- Enode 1 address:
enode://ac95810828228259627098da243875478144658d15025f6f18739ef81b6b0b2889d2cb0c2df15d6abe001165e6df2dc556eac572ff437eea17479fc653719b48@100.11.141.79:30303

**Node 2**
- Password: access2
- Public address: 0xAFD42957b680BfF188D98CE8d40BA794AbBf946A
- Enode 2 address:
enode://5816b76c8934383a83e8489d5444274f8390f13b08bb7b67fb80a69abdfb0f765dbab46c9c7a23de68f6a8719b102a2f2bb5de663fc5d7defbbcd22e2ff85773@100.11.141.79:30304









