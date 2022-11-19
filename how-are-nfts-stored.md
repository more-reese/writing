Published with [PubDAO](https://pubdao.co/) on Decrypt, August 2022
# How Are NFTs Stored? On-Chain, Off-Chain and Decentralized Storage
The data that makes up the content of NFTs needs to be stored somewhere—but not all NFT storage techniques are created equal.

Non-fungible tokens (NFTs) are, ultimately, a form of digital media. And just like other digital media—from the words written in Decrypt articles to YouTube videos and streamed music—NFTs, in their most basic form, consist of data made up of 1s and 0s.

That’s important because everything associated with the NFT—from the smart contract it lives in to the URL you use to view it to the image itself—ultimately boils down to 1s and 0s that are stored on a computer.

Not all NFT storage techniques are created equal, however. Indeed, some NFT holders may not own much more than a URL or token ID. So it's worth taking the time to understand how NFT storage works before you think about buying or making an NFT.

Before we dive in let's take a look at some core concepts:

- 🖥️ Servers—A server is a computer, just like the one you're reading this article on. Unlike the computer you're reading this on, however, servers are exceptionally powerful and can run many different programs simultaneously. At their root, NFTs live and are stored on servers.
- 🖧 Hosting—The vast majority of people do not run their own servers so, whether they realize it or not, they rely on someone else to provide that service. Hosting refers to a collection of services, including storage, typically run on servers. All NFTs are hosted somewhere.
- 💽 Metadata—Metadata is data that describes other data. Metadata helps servers find, process, and store data more efficiently. The metadata of an NFT describes characteristics like (for a PFP NFT) its name, color, size, shape, hat type, glasses type, etc
- #️⃣ Hash—A hash is a cryptographic function that, given some input, produces the same output every time. A hash is typically used to encode and a lot of information verifiably and efficiently. An NFT and all its metadata can be stored in a single hash. To get hands on experience with hashing, check out this hash generator.
- 📝 Smart contract—Smart contracts are encoded instructions that live on a blockchain. They are the building blocks of decentralized applications (dapps), including most NFTs. The rules for minting and exchanging NFTs live in smart contracts.

# On-chain vs off-chain storage
Storing an NFT on-chain means that the entire NFT—the image and all its metadata—exist on a blockchain. Conversely, off-chain stored NFTs means that some or most of the NFT is stored outside of the blockchain.

On-chain storage can be preferable because it means that users can verify all facets of the NFT. However, very few NFT projects opt for this method of storage.

An example of one that does is Autoglyphs. The reason for this is simple—JPEG images contain a lot of data, especially when those images exist in collections on the order of thousands or tens of thousands.

As a result, most NFT projects opt to store the actual images off chain. Many well known NFT projects like CryptoPunks and Bored Ape Yacht Club opt for off-chain storage.

# Centralized vs decentralized hosting
In the case of off-chain storage, the NFT's smart contract contains information that points to some off-chain location where the actual NFT JPEG image is stored. Often, the NFT image and its metadata are stored in a hash.

This hash is used to point to either a centralized or decentralized hosting provider.

Examples of centralized hosting providers include Amazon and Google. Centralized hosting providers run servers that store the 1s and 0s that make up the NFT.

The risk of centralized hosting providers is that (although unlikely) they could shut down at any time and the owner’s NFT would be lost. All the owner would be left with is, in some cases, as a simple hash that exists in a smart contract.

That is why many projects opt to use decentralized solutions to host their NFTs. The most common solution is to host NFT data on the InterPlanetary File System (IPFS). IPFS is a distributed peer-to-peer network on which files are stored across multiple nodes, making them resistant to single points of failure such as server issues.

While NFTs stored on IPFS are not technically stored on-chain, they are theoretically safer because IPFS is censorship-resistant; no single entity has the power to shut it down.
