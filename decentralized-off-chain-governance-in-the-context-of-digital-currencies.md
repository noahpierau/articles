# Decentralized off-chain governance in the context of digital currencies
Digital currencies such as Bitcoin, Monero, Zcash or Decred aim to operate in a decentralized way. In practice, this means that there is no central control over their public blockchain. However, off-chain governance processes still need a platform where contributors can come together and collaborate. In many decentralized projects the question arises: *how to organize off-chain governance in a robust and decentralized way*?

## Case study: GitHub
This article will start with a short case study on the usage of GitHub as the primary governance platform of the Zcash Foundation. It uses observations and comments from [this GitHub issue](https://github.com/ZcashFoundation/ZcashFoundation/issues/58).

The starting point was the observation that non-programmers seem to have a problem with using GitHub as a governance platform:

>“I was interested in this Zcash community and governance thing, but then I tried to join in but it was on GitHub, so I gave up”

and:

>“Oh yeah, I tried to look into that thing, but it was on GitHub and I can never find anything on GitHub.”

Funny quote from the comments:

>Trying to bring non-programmers into GitHub is like trying to create a cypherpunk community on Facebook.

It was added that educating people before they can engage is generally not very likely to be successful. People often neglect educational materials, or they may be uninterested in learning the required skills.

More importantly, GitHub is banned in countries such as China.

In order to engage people with diverse backgrounds, it should be possible to participate in off-chain governance processes via platforms that are different from GitHub (or Facebook!). This includes getting in touch, interacting with the community, contributing work, and exercising power.

## How to organize off-chain governance
It is important to consider who to include into what. There are several levels of participation. Higher levels naturally have higher barriers.

### Level 1: get in touch

To onboard people and help them out, chats work just fine: Slack, Discord, Matrix, RocketChat, IRC and such. Casual platforms like Twitter and Facebook also fit. Most superficial conversations are level 1 governance.

### Level 2: interact with the community

Next, when people get around and have something to say, they have a choice. If it’s something quick and not too important they can use chat. If they want to start a thoughtful discussion that won’t drown in history, it’s better to use something topic-based: GitHub, Reddit, forums, or mailing lists.

Commenting on GitHub issues, Reddit threads, or forum posts is no more difficult than responding on Twitter or Facebook. Login, search, click, enter text, submit: these are trivial actions. If a person has the skills to understand and take part in discussions around projects such as Bitcoin, Monero, Zcash, or Decred, they can surely handle GitHub or Reddit.

### Level 3: contribute work

An even higher level is if they have work to contribute: a good idea, a bug report, code, design, and so on. A platform similar to GitHub is necessary at this level, since you need an issue tracker to work more effectively.

### Level 4: exercise power

The highest level is exercising power. This is “serious” governance. This level demands more from the people and the platform in use.

Participants must know what they are doing. They need relevant information to understand the items currently on the agenda. Since their decisions will impact the future of a digital currency, ideally they are aligned with the project through *skin in the game* — reputation or wealth to lose.

The platforms used to exercise power (submitting, reviewing and voting on proposals) must satisfy special requirements:

*    Version controlled documents and databases.
*    Data is timestamped and signed to verify integrity.
*    Decentralization: the platform must survive shutdowns with no data loss and minimum time to recover (easy to replicate).
*    It must be *very* expensive to overwrite content, which is achieved by anchoring data into a secure public blockchain.
*    Sybil-resistant voting system to make collective decisions.
*    Payment barriers to register and submit proposals. Note, we’re talking about small amounts to combat [sockpuppets](https://en.wikipedia.org/wiki/Sockpuppet_%28Internet%29) and spam.
*    Balanced approach to malicious behavior. Transparent, publicly provable censorship to strip outright spam, and at the same time prevent silent censorship like on Twitter and Reddit.
*    For proposals funded by digital currencies: ideally, disbursements are automated and control is decentralized.

Satisfying all these requirements can be tricky. However, if the aim is to organize off-chain governance in a robust and decentralized way, it is necessary to mitigate as many attack vectors as possible.

## Existing level 4 governance platforms

There is an existing off-chain governance platform called Politeia that meets most requirements listed above. It is being built by Decred, a project that explores governance all the way down the rabbit hole.

While the Politeia platform is already in use, it is actively being developed since the project is taking an iterative approach. The level 4 requirement that is still missing is the “automated disbursement of funds” part, but it is planned for release in the foreseeable future.

Politeia is an open source project. Most of the Decred-specific code is designed as a plugin or config setting. It could be customized for Zcash: anchor data into the Zcash blockchain, use a Zcash block explorer, use ZEC for paywalls, fund proposals from a Zcash Foundation address, and so on.

Moreover, any organization that wants to run their own Politeia instance on top of Decred in order to get the benefits of a versioned, timestamped and blockchain anchored governance platform is free to do so. In fact, it is generic enough to support many [use-cases](https://btcmanager.com/decreds-politeia-challenge-overview-winners/).

There are also Ethereum-based projects that are working on governance platforms. Some notable examples include Aragon, DAOstack, and Colony. Another interesting initiative is Moloch, which seems to be somewhat similar to Vitalik’s DAICO. However, it remains to be seen if these projects will deliver all the level 4 requirements listed above.

## Conclusions

Most digital currencies such as Bitcoin, Monero, Zcash or Decred operate in a decentralized way via public blockchains, but off-chain governance often makes use of centralized platforms (GitHub) where contributors come together and make decisions about the future of the project.

This article has examined how off-chain governance can be organized in a robust and decentralized way. People with diverse backgrounds prefer a wide range of different platforms. Similarly, the four levels of governance require different forms of participation. For these reasons, it is wise to embrace multiple platforms for off-chain governance.

When it comes to exercising power — serious governance — both the people and the platform are important. Governance participants should have access to relevant information and skin in the game, while the platform should be designed to mitigate as many attack vectors as possible.

Ultimately, there are no “one size fits all” solutions. Each project could pick a unique mix of governance platforms, tailor-made for their community.

***

Originally published via: https://blog.goodaudience.com/decentralized-off-chain-governance-in-the-context-of-digital-currencies-ef6db7d97412
