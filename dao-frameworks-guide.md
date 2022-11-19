Published with [Content Guild](https://www.tally.xyz/gov/eip155:137:0x26217Ec5044AEB8D6495BC68eE91951cd7Bb02a0) on [Tally official blog](https://blog.tally.xyz/a-pocket-guide-to-dao-frameworks-8d7ad5af3a1b), October 2022

# A Pocket Guide to DAO Frameworks
### An introduction to the essential on-chain infrastructure that helps run today’s biggest DAOs

# What is a DAO framework?

Frameworks are structures around, in, and on which things are built. The structures that frame the things take some cogent and mutually agreed upon form (e.g., rules, laws, guidelines).

DAOs are coordination frameworks for humans and computers to do things together on the Internet. DAOs frame how humans use blockchain technology to coordinate decisions that pertain to community and capital.

A DAO framework defines the specific set of structured interactions that humans and smart contracts use to make and execute decisions in service of the DAO’s purpose. Essential to any DAO framework are the governance frameworks and processes it employs.

Part of what the “A” in DAO implies is that the organization will persist and community-approved decisions will execute autonomously on-chain irrespective of the DAO’s membership makeup. As Vitalk Buterin wrote in 2014:

“a [DAO] is…an entity that lives on the internet and exists autonomously, but also heavily relies on hiring individuals to perform certain tasks that the automaton itself cannot do.”

This is what makes DAO frameworks and the governance processes that they run so important; they are organizational design patterns for building and upgrading autonomous, blockchain-based organizations composed of people and code.

Projects that have a 4/7 (at best) multi-sig and use Snapshot for polling may call themselves DAOs. But how can such organizations persist autonomously when so much happens off-chain and decision execution depends upon a small group of trusted humans?

The question above is not intended to criticize such projects. It is, however, intended to illuminate what, in a final analysis, may be perceived as a disingenuous representation of a Decentralized Autonomous Organization. In order for DAOs to grow into their full potential, we need some convergence around standard definitions and agreed upon frameworks.

The rest of this piece looks at some of the most popular DAO frameworks available today, as well as the governance frameworks and processes that underpin them.

# OpenZeppelin Governor
### A DAO framework for modular on-chain governance

OpenZeppelin is an open-source framework to build and operate secure blockchain applications. Their work is essential infrastructure for the Ethereum ecosystem and is trusted by blue chip projects like Aave, Optimism, and Compound.

This “blueprint for decentralized” systems is centered around OpenZeppelin’s two core products for building on Ethereum. Contracts is a library of modular, reusable secure smart contracts in Solidity, and Defender is a security operations platform that helps teams ship secure applications quickly (source). Both products, reviewed and battle-tested by the wider Ethereum community, contain primitives that open new possibilities for DAOs on-chain. One such primitive is OpenZeppelin Governor.

In August 2021, OpenZeppelin announced a new secure, modular system for on-chain governance: OpenZeppelin Governor. Developed in collaboration with Compound, and drawing on their pioneering governance tools, the OpenZeppelin Governor contracts release marked a milestone in the path toward decentralized governance on-chain.

## Modular Governance On-Chain
OpenZeppelin Governor’s ingenuity is in its modular system design. Core to this design are two required modules: Votes and Counting.

Votes is where voting power comes from. Voting power, or weight, can come from a few places. First is from an ERC20Votes token, which specifies things like voter account and any delegates delegating their voting power to said account. Second is from ERC20VotesComp, which supports Compound’s voting and delegation. Third is from GovernorVotesQuorumFraction, which draws from ERC20Votes token but also specifies a quorum.

Counting is where user voting options are set and define how votes are counted. A user can vote for, again, or abstain from voting. If a quorum is set, “for” and “abstain” votes count toward quorum but “against’’ votes don’t.

Key to the Governor system’s modularity is its suite of extensions. For example, a timelock allows for a delay between when a proposal passes and when it is executed. A threshold sets the minimum number of votes required to create a proposal. You can learn more about the full set of extensions here.

## OpenZeppelin Governor in the Wild
OpenZeppelin’s Wizard makes it easy to interact with and customize the Governor contract to set up DAO governance. Users can set required parameters around voting and counting, as well as optional parameters like timlelock and threshold.

Through its intuitive user-interface Tally, a core OpenZeppelin partner, makes it easy for DAO members to navigate proposals, cast votes, and visualize voting power.

If you want to join the ranks of major projects like ENS DAO and Nouns DAO and start using OpenZeppelin Governor for your DAO, check out Tally’s onboarding guide.

# Moloch
### A minimum viable DAO framework

Moloch is a DAO framework conceived as an idea for a “minimum viable DAO”. The minimum viability is straightforward: streamline grants in order to get value-adding developments funded faster (source).

Launched on Valentine’s Day 2019, the aptly named Moloch DAO was first to implement the Moloch framework and run on its set of smart contracts. Moloch DAO exemplified “minimal viable DAO” by focusing on grant giving to projects that furthered the then-somewhat-stagnant development of public infrastructure for the Ethereum 2.0 ecosystem.

The original Moloch smart contract, which impressively was less than 600 lines of code, was optimized to balance community-driven decision making for capital aggregation and allocation, with an individual’s agency and right to reclaim their portion of the treasury should they disagree with the community’s decision. This novel governance mechanism, Ragequit, acted as an on-chain opt-out clause for DAO contributors.

## Minimum Viable Governance
Moloch V1’s minimum viable DAO governance process works like this:

### Proposal Submission

Only DAO members can submit proposals. There are two types: 1) the Membership proposal for deciding which new DAO members to accept/reject and, 2) the Grant proposal for deciding which projects to give grant funding. Proposals are capped at five per day.

### Voting Period

The Voting Period is 7 days. Members get one vote each. Votes are won by simple majority with no quorum on the required number of votes. At the end of 7 days, votes are counted and finalized but, importantly, the result is not processed on-chain.

### Grace Period

The Grace Period commences at the end of the Voting Period after the votes are finalized. It lasts 7 days. During these 7 days, members who voted “No” have the right to Ragequit should they disagree with the vote’s outcome. Upon exercising this right, a member receives their portion of the treasury but also foregoes their DAO membership.

The vote’s outcome is executed and processed on-chain at the end of the Grace Period.

If you’re interested in more detail on Moloch’s minimum viable governance process and other aspects of the framework, such as membership types and its anti-collusion mechanism, check out the whitepaper.

## Moloch V2 & V3
Since 2019, the Moloch framework and its set of smart contracts have undergone two major upgrades: Moloch V2 in March 2020 and Moloch V3 (aka “Baal”) in February 2022.

While the minimum viable DAO ethos persists, the upgrades make the Moloch framework more extensible and flexible. Key governance process improvements include:

- More detailed proposal and voting process (e.g., open proposal submission)
- GuildKick to pass to vote on removing malicious members
- Boosts to integrate with external apps like Discord or Snapshot
- Minions to interact with external smart contracts
- Privileged roles to do things like cancel a proposal and configure membership

Read more on Moloch V2 here and V3 here.

## Moloch DAOs in the Wild
Today there are over 800 DAOs using the Moloch framework, including The Lao, MetaCartel Ventures, and Raid Guild. You can explore the Moloch ecosystem with DAOhaus, a no-code platform for creating and managing Moloch DAOs.

# Aragon
### A DAO framework for a global network of DAOs

To call Aragon solely a DAO framework is overly reductive. Certainly, Aragon is a DAO framework. But it is also an expansive platform for DAO builders. Since its 2017 whitepaper, which described Aragon as, “a dApp that lets anyone create and manage any kind of organization (companies, open source projects, NGOs, foundations, hedge funds…) on the Ethereum blockchain,” the Aragon Network and community has since built a robust ecosystem of tools, applications, and services for creating a cryptonetwork for decentralized organizations to thrive (source).

An exhaustive elucidation of the Aragon Network, platform, and ecosystem is beyond the scope of this piece. Suffice it to say, however, that it includes a suite of solutions for everything from APIs to frontend applications that developers and non-developers alike can use for all things DAO. We’ll focus on one specific solution, Aragon Govern, and the novel governance framework that it is built around.

## Optimistic Governance
Aragon employs a unique governance framework that assumes all proposals will pass unless indicated otherwise. This type of governance, called Optimistic Governance or “lazy” governance, defaults toward executing proposal transactions on-chain unless they are otherwise challenged. One of the biggest benefits of Optimistic Governance is that DAO members avoid the pervasive DAO problem of voter fatigue or burnout.

Aragon’s Optimistic Governance framework structures how proposals pass through the DAO using the Govern set of smart contracts and is arbitrated by Aragon Court. In the framework, DAO members can submit a proposal with a scheduled execution. An in-built delay period gives Court Guardians time to review the proposal.

If the proposal passes, its execution is available and the on-chain transaction occurs at the scheduled execution time. If the proposal is challenged, a dispute is created and Guardians are drafted. The proposal goes through a series of dispute stages and Guardians re-vote on it. If majority approves, the execution is available and the on-chain transaction occurs at the scheduled execution time. If it fails, the execution is canceled.



Compared to Moloch’s minimum viable governance framework, Aragon’s Optimistic Governance framework requires less operational overhead from a DAO member perspective. However, the initial set up is less “out of the box” than Moloch’s given the parameters builders must set when setting up an Aragon DAO.

All of the above does come with a caveat though.

## Aragon App
In April 2022, Aragon announced plans to rebuild its foundation. Under construction at the time of writing, Aragon App seeks to integrate its existing solutions into a single experience and design system that makes it easy for any builder to create and run a DAO. This does not mean solutions like Govern and Court will go away. Instead they will operate “under the hood”. The Aragon team has not published any timelines on the release of Aragon app, but you can keep up to date on the App website.

## Aragon DAOs in the Wild
To date over 3,800 DAOs have been built with Aragon (source). Some of the more notable ones include decentralized oracle API3, metaverse Decentraland, and social identity network BrightID.

# Other DAO Frameworks
OpenZeppelin Governor, Moloch, and Aragon only scratch the surface in this nascent and rapidly evolving space. An unexhaustive list of other DAO frameworks, platforms, and tooling systems includes: Colony, Tribute, OpenLaw, Syndicate, DAODAO, FactoryDAO, XDAO, Astro, DAOstack, Metropolis (formerly Orca Protocol), KALI, Metaphor.xyz, Upstream Collectives, and many more.

