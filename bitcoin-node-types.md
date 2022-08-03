Published with (PubDAO)[https://pubdao.co/] on [Decrypt](https://decrypt.co/resources/what-are-the-different-types-of-bitcoin-nodes-how-the-bitcoin-network-is-maintained), July 2022

# What Are The Different Types of Bitcoin Nodes? How the Bitcoin Network is Maintained
### The underlying infrastructure of the Bitcoin network is secured and maintained by nodes—find out what they are, and how they work.

Bitcoin nodes are the underlying infrastructure of the Bitcoin network, securing and maintaining it. But despite their importance, Bitcoin nodes are often misunderstood or not understood at all.

In this article, we’ll explore what Bitcoin nodes are, as well as the different types of Bitcoin nodes and their role in the Bitcoin network.

## What is Bitcoin?
When most people say "Bitcoin" they are referring to Bitcoin the cryptocurrency. But Bitcoin is more than that:

- Bitcoin is a network; it is a collection of interconnected computers that share information.
- Bitcoin is a protocol; it is a set of rules for how information can be shared on the network.
- Bitcoin is software; it is a computer program that knows the protocol rules and is run by computers on the network so that they can share information with each other.

Using the same word to describe different (although certainly related) things can be confusing. For the sake of this piece, we'll use the following terms to refer to the different uses of "Bitcoin":

- BTC describes Bitcoin the cryptocurrency, that people buy, sell, and trade.
- Bitcoin software describes the Bitcoin protocol rules that are encoded into a language computers understand, allowing them to use to connect and share information about BTC transactions.
- Bitcoin network describes the network of interconnected computers, each of which runs its own version of the Bitcoin software.

These differentiations provide helpful context for explaining the different types of Bitcoin nodes. Before discussing Bitcoin nodes specifically, it’s worth briefly discussing at a high level what nodes are.

## What are nodes?
In general, a node is a point on a network. For example, a car is a node on a network of highways, or a work colleague a node in a professional network.

In the world of computers, nodes are devices connected to a computer network that transmit, process, and store information.

Nodes consist of two things: hardware and software. Hardware is the physical stuff—microchips, processors, etc—required to run software. Software is a set of instructions that can be stored and run by hardware.

For example, your smartphone is a node on the internet. The apps you run (browsers, messaging apps, maps, etc) are pieces of software that can connect to the internet and give it instructions for what type of information to send, receive, and store (such as websites, text messages, and directions). These instructions and pieces of information are processed and stored on tangible pieces of hardware that are inside your phone and other computers connected to the internet.

Compared to the internet and cell phones, the Bitcoin network and Bitcoin nodes are extremely simple. While the internet and cellphones are designed to transmit and store all sorts of information, the Bitcoin network and Bitcoin nodes are designed to transmit and store one type of information—data representing BTC transactions.

## What are Bitcoin nodes?
Bitcoin nodes are computers that run Bitcoin software and are connected to the Bitcoin network. Bitcoin nodes validate, broadcast, process and store BTC transactions.

BTC transactions are batched and stored into groups called blocks. This is where the term blockchain comes from—historical transactions stored in blocks that are linked together. Before a block is added to the blockchain, nodes must verify that the block's transactions are valid.

This verification involves checking things like whether the same BTC was spent twice, or whether a sender actually has the BTC they are trying to send. The process of individual nodes collectively agreeing upon the validity of a block (and the transactions it contains) before adding it to the blockchain is known as consensus.

Because Bitcoin is a peer-to-peer payment system, it does not have intermediaries or middlemen to enforce consensus rules on the Bitcoin network. Therefore, nodes must achieve consensus amongst themselves. They do this using the Bitcoin software.

In addition to the Bitcoin protocol rules, the Bitcoin software contains a full copy of the Bitcoin blockchain. So, when a node downloads the Bitcoin software and connects to the Bitcoin network, it has the same transaction history and works off of the same set of rules for verifying transactions as every other Bitcoin node. This way, when a new transaction is broadcast to the network, each individual node does its own work to check a transaction's validity.

Similarly, when a new block is broadcast to the network, each node decides whether or not to add it to their copy of the blockchain. This design allows for nodes to trustlessly verify BTC transactions and blocks.

## Types of Bitcoin nodes
A helpful frame for understanding the different Bitcoin node types is, what role does the node play in adding blocks to the blockchain?

## The main types of Bitcoin nodes
Remember, Bitcoin nodes broadcast, validate, process, and store BTC transactions—and blocks are collections of valid BTC transactions.

### Full node

When a transaction occurs, a full node picks it up. Full nodes store the entire blockchain and can fully verify all rules of the Bitcoin network using the Bitcoin software. A full node checks the transaction's validity against the blockchain history and the set of rules encoded in the Bitcoin software.

If the transaction is valid, the full node broadcasts it to other nodes it's connected to. These nodes go through the same verification process. Once a sufficient number of full nodes agree the transaction is valid, it’s added to a pool of other valid transactions.

### Miners

Mining nodes, or miners, pick up transactions from this pool and package them into blocks.

Miners run a version of the Bitcoin software that contains special rules for creating and proposing blocks to the Bitcoin network. This includes things like how big a block can be, how to format transactions, and how to sign a block.

Miners compete against one another in a race to create the next block. Once a miner thinks it has created a valid block, it broadcasts the proposed block to other nodes on the Bitcoin network.

Full nodes pick up the block and, in a similar manner to how they validate a single transaction, they verify the validity of the block according to the rules encoded in the Bitcoin software they are running. If a full node considers a block valid, it adds the block to its respective copy of the blockchain, broadcasts it to the Bitcoin network and other nodes go through the same verification process.

Once a sufficient number of nodes validate the block and add it to their copy of the blockchain, consensus is reached. At this point, the transactions in the block are processed, all nodes verify and store the updated version of the blockchain, and miners begin the race to create the next block.

### Mining: Full nodes vs miners

Miners are incentivized to create and propose valid blocks because the miner whose block is added to the blockchain receives a reward. This block reward consists of newly minted BTC pre-programmed into the Bitcoin software, plus BTC-denominated fees for all the transactions contained within the block.

Mining is competitive and expensive. If a miner proposes an invalid block (for example, with false transactions), the block is rejected by other nodes and the miner isn't rewarded for the time and money spent to create the block. Therefore, miners are incentivized to propose valid blocks only.

A key difference between full nodes and miners is that miners can propose new blocks to the Bitcoin network and full nodes cannot. By extension, miners can receive block rewards while full nodes cannot.

The resource intensity of mining means that miners must use specialized, powerful hardware designed specifically to create and propose new blocks. By contrast, full nodes can run on most laptops, and even a Raspberry Pi.

This brings us to the third and final primary type of Bitcoin node—light nodes.

### Light nodes

Light nodes run a special version of Bitcoin software that stores, as the name implies, a lightweight version of the blockchain. This version of the blockchain contains block headers, which are codes in each block that basically say “this block is valid”. This allows light nodes to connect to and transact on the Bitcoin network, without the need to store its full history.

Importantly, however, this means that light nodes cannot independently verify the Bitcoin network rules and, therefore, must connect to full nodes in order to get the block data.

Mobile wallets are the most common example of light nodes. Most mobile phones (with one or two exceptions) aren't powerful enough to run a full node, and are certainly not powerful enough to run a miner. But they are powerful enough to store a compressed version of the blockchain with information about wallets address BTC balances. If you've sent or received BTC from your phone, your device is a node on the Bitcoin network!

## Other types of Bitcoin nodes
Full nodes, miners, and light nodes are the main types of Bitcoin node. However, there are some other types of node that are frequently mentioned, and warrant descriptions.

- ⚡ **Lightning nodes**: Lightning is a network built on top of the Bitcoin network so that people can transact BTC faster and cheaper. Lightning nodes coordinate this activity.
- 🗄️ **Archive nodes:** Also known as full archival nodes, archive nodes are synonymous with full nodes; they store a full copy of the blockchain and can verify all Bitcoin network rules. The differentiation stems from the fact that people sometimes break full nodes into two types—archive nodes and pruned nodes.
- ✂️ P**runed nodes:** Pruned nodes store the full blockchain history up to a certain size. Once this size limit is met, they begin deleting or pruning earlier blocks so that they can store full versions of new blocks. Pruned nodes are smaller than full nodes but bigger than light nodes.
- ⛏️ **Mining pool nodes:** Mining pool nodes orchestrate mining activity from groups of miners so they can pool resources to mine new blocks. When a mining pool node creates a block that is added to the blockchain, the node distributes the block reward to miners proportionate to their amount of resources. Miners like mining pools because it means they get paid more consistently. For example, instead of getting 10 BTC every 100 blocks, they could get 1 BTC every 10 blocks

## Summary
Bitcoin nodes are computers connected to the Bitcoin network that run Bitcoin software in order to broadcast, validate, process, and store BTC transactions and blocks. There are three main types of Bitcoin nodes.

- **Full nodes** trustlessly validate transactions and blocks in order to achieve consensus on the transaction history. In this way, full nodes ultimately decide which blocks get added to the block.
- **Miners** organize transactions into blocks that they then propose to the Bitcoin network. If a miner’s block is added to the blockchain the miner gets the block reward. In this way, miners facilitate newly minted BTC coming into circulation.
- **Light nodes **store a pared down version of the Bitcoin blockchain by connecting to full nodes. In this way, light nodes allow for BTC transactions on low power devices like mobile phones.
