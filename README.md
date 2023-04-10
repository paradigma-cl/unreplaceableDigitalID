# unreplaceableDigitalID
## Your Digital ID or the Digital ID of your organization must be unreplaceable.  
### prepared by CrossCheck-Paradigma
Your Digital ID or the Digital ID of your organization must be unreplaceable.  We must enjoy a secure world, peaceful, and without setbacks produced by hackers or identity theft.

DNS and social media are based on the Internet domain name system, names are globally unique and human-readable, but not strongly owned. The system operator has the final say as to what each name resolves to.  This requires that client must trust the system, and trust that the administrators are the only ones that can make these changes.
In PGP, names are key IDs.  PGP is short for Pretty Good Privacy, a security program that enables users to communicate securely by decrypting and encrypting messages, authenticating messages through digital signatures, and encrypting files. They are globally unique and cryptographically owned, but not human-readable. PGP key IDs are derived from the keys they reference. But these names are difficult for most users to remember since they do not carry semantic information relating to their use in the system.
## Solution
[BNS](https://docs.stacks.co/docs/stacks-academy/bns) names have all these properties, and none of these problems. This makes it a powerful tool for building all kinds of network applications. Using the BNS, the following can be achieved and more:
- Build domain name services where hostnames cannot be hijacked.
- Build social media platforms where user names cannot be stolen by phishers.
- Build version control systems where repository branches do not conflict.
- Build public-key infrastructure where it is easy for users to discover and remember each other's keys.

Software applications built with the Stacks blockchain integrated, give users control over their digital identities, assets, and data. Unlike most cloud-based apps, they are "decentralized" since they do not depend on any centralized platform, server, or database to function. Rather, they use the Stacks blockchain to authenticate users and facilitate read and write requests for them without any single point of failure or trust.

The Stacks blockchain addresses performance problems using a layered approach. The base layer consists of the Stacks blockchain, and the Blockchain Naming System (BNS). The blockchain governs ownership of identities in the Stacks network. Identities can be names such as domain or subdomain names, or application names.
Decentralized Applications (Dapp’s) is the New App that integrates these main functions, authentication, transaction signing, and data storage. All users can run their applications under their own private decentralized space. Each user has access to and/or shares with other users its own private data through the decentralized application. 
These domain or subdomain names are called decentralized names or decentralized IDs, and they are registered to the public key associated to its private key or address, through a name registry implemented in a smart contract on Stacks, secured by Bitcoin.  The provable smart contract is written in Clarity, a safe, decidable language. The contract links the STX address and the username according to the rules about fees and expiry.

Names in BNS have four properties:
- Names are globally unique. The protocol does not allow name collisions, and all well-behaved nodes resolve a given name to the same state.
- Names are human-meaningful. Each name is chosen by its creator.
- Names are strongly owned. Only the name's owner can change the state it resolves to. A name is owned because the owner of its private key can generate valid transactions that update its zone file hash and ownership. The name zone file can only have a valid verification using the owner’s private key.
- Names using its associated public and private key can sign transactions.  Only the owner of the name and the associated keys can sign in a verifiable way transactions, and the execution of the smart contracts in a decentralized way. This action represents the unique action of a user, that has access to those keys.

### 1.	Blockchain network interoperability
A user private and public keys are based from the mathematical, and cryptographical algorithm, and they are base to use it in the Stacks or Bitcoin blockchain.

From a private key the user can derive a decidable public key in a Stacks address format, and in several Bitcoin addresses format.  A Stacks address starts with a “SP”.  Initially, the Bitcoin address was based on the legacy address P2PKH starting with a “1”, the actual ones are based on SegWit address P2WPKH starting with a “bc1”, and Taproot address when massively available starting with a “bc1p”.  These addresses are mathematically or cryptographically linked together as one or the same, but they are used in the Stacks or Bitcoin blockchain ecosystem respectively.

The Stacks blockchain ensures that each node's BNS view is synchronized to all of the other nodes in the world, so queries on one node will be the same on other nodes. Stacks blockchain nodes allow a name's owner to bind up to 40Kb of off-chain state to their name, which will be replicated to all other Stacks blockchain nodes via a P2P network.

The biggest consequence for developers is that in BNS, reading name state is fast and cheap but writing name state is slow and expensive. This is because registering and modifying names requires one or more transactions to be sent to the underlying blockchain, and BNS nodes will not process them until they are sufficiently confirmed. Users and developers need to acquire and spend the requisite cryptocurrency (STX) to send BNS transactions.
At another level, the different applications could interact among them exchanging information. In order to use these capabilities, a set of standard verifiable digital identities should be used integrated into the web to have a secure and private interaction.

### 2.	Definition of a publicly accessible app’s profile and app user’s profile
The Stacks zone files have the capabilities, and the tools to define the profiles for the application itself, and each of its users, depending on the application to identify its subjects, in a decentralized way using the Internet.

The W3C (https://www.w3.org) recommends Decentralized identifiers (DIDs), as a new type of identifier that enables verifiable, decentralized digital identity. A DID identifies any subject (e.g., a person, organization, thing, data model, abstract entity, etc.) that the controller of the DID decides to identify. In contrast to typical, federated identifiers, DIDs have been designed so that they may be decoupled from centralized registries, identity providers, and certificate authorities. DIDs are URIs that associate a DID subject with a DID document allowing trustable interactions associated with that subject. Each DID document can express cryptographic material, verification methods, or services, which provide a set of mechanisms enabling a DID controller to prove control of the DID.

The DIDs for a person for example, are expressed through a name and an image, sometimes a description, background image, url, etc. The visual and textual representation of an account, helps users to better recognize own accounts and accounts of other users. Stacks has a long history of Decentralized Identifiers (DIDs) as they introduced human readable names for bitcoin addresses when the project started as “One Name” back in 2014.

The Stacks public DIDs is a profile that is registered with a username on-chain using the BNS (Blockchain Naming System) smart contract. These profiles are defined using the JSON web token, and its contents using the appropriate objects of the Schema standard (https://schema.org), like the person object (https://schema.org/Person).

#### 2.1 BNS and DID Standards
BNS names can be compliant with the emerging Decentralized Identity Foundation (identity.foundation) protocol specification for decentralized identifiers (DIDs), and the W3C foundation. These initiatives define mechanisms by which an End-User can leverage an open provider to release identity information (such as authentication and claims) to a Relying Party which can act on that information.

Each name in BNS has an associated DID. The DID format for BNS is:
- did:stack:v2:{address}-{index}
- did:btc-addr: {address}-{index}

Where:
- {address} is an on-chain public key hash (for example a Stacks or Bitcoin address).
- {index} refers to the nth name this address created.

#### 2.2 Using the Internet domain names to verify decentralized domain and subdomain names
To incentivize mass adoption of DIDs, one initial strategy is to link both Internet Domain Names to DIDs, both referring to each other, in the BNS zone file a reference to a web server, and in the Internet domain server referring to the respective DID.  Mixing a centralized domain names with the decentralized domain names. For example, the Internet domain name XCK.app refers to the Stacks DID XCK.app, and both are owned by the same controller. In this case, the controller should be the dapp.

This strategy is ratified by a recent proposal in using a new DID method in conjunction with blockchain-based DIDs that allows them to bootstrap trust using a web domain's existing reputation (https://w3c-ccg.github.io/did-method-web).

#### 2.3 Extending the naming characters for the domain and subdomain names
Typically, the domain and subdomain names have commonly used Latin characters in ascii format.  Due to the convergence of the use of different languages, and character systems, the popularity in social apps, people have started to think about using emoji as names for their domains or subdomains.  The compatibility of the dapps with Punycode could be a facilitator of mass user adoption.
For example: 🧑‍💼 .xck.app is represented as xn-- -zc3sr5i.xck.app

### 3.	The App Profile
Each App (web application) should have a verified identity in order to safely reference it and be trustworthy of interaction between other applications.
An app can be identified both by the Internet domain (DNS) for example 'XCK.app' and the Stacks DID 'XCK.app' In case, it is a web application, it could be accessed as https://xck.app having both definitions.

The description for an App Profile document is done using a JSON web token based on the WebApplication Schema object (https://schema.org/WebApplication).
Additionally, this App Profile document must include the did-method-web. The example is represented as 'did:web:xck.app'. The target system of the Web DID method is the web host that the domain name described by the DID resolves to when queried through the Domain Name System (DNS). This did-method-web is included in this app profile.

It could be useful to have a way to retrieve a verifiable DID profile for the Aspp as recommended by the W3C using an URI. For example, a web URI https://xck.app?profile
In this case, the application should also return a JSON web token using the protocol previously mentioned.

Example of the WebApplication JSON web token included in the profile for 'XCK.app'

#### 3.1 The App did:web DID document
Creating a DID is done by: applying at a domain name registrar for use of a domain name and storing the location of a hosting service, the IP address at a DNS lookup service creating the DID document JSON-LD file including a suitable keypair, e.g., using the Koblitz Curve, and storing the did.json file under the well-known URL to represent the entire domain.

For example, for the domain name 'xck.app', the 'did.json' will be available under the following URL: 'did:web:xck.app' -> https://xck.app?did.json

Example of the 'did.json' file for 'XCK.app'

Expanding the Internet Domain Names to the users Decentralized Identifiers

For the users of each App (web application), the App could provide a verified user identity in order to safely reference across other applications.
In this context, the DIDs are URIs that associate a DID subject as a user of the application with a DID document allowing trustable interactions associated with that subject.

#### 3.2 The App User's Profile document
The Stacks Blockchain Name System has the possibility to create subdomain names under a defined decentralized domain name. A user can claim a subdomain name, having the attribute of a DID. Using the same example, for the user 'support', the subdomain name is 'support.xck.app'

In the example used here, the user is identified by this subdomain name, and it could be useful to retrieve a verifiable DID profile for the App User as recommended by the W3C using an URI. For example, a web URI https://support.xck.app?profile

The description for an App User Profile document is done using a JSON web token based on the Person Schema object (https://schema.org/Person).

Also, this document has to include the did-method-web for the app user. For the user support.xck.app as an example, it is represented as 'did:web:support.xck.app'. The target system of the Web DID method is the web host that the domain name described by the DID resolves to when queried through the Domain Name System (DNS). This did-method-web is included in this app user profile.

In this case, the application should also return a JSON web token using the Person Schema object.

Example of the Person JSON web token included in the profile for support.XCK.app

#### 3.3 The App User did:web DID document
Creating a DID is done by: applying at a domain name registrar for use of a domain name and storing the location of a hosting service, the IP address at a DNS lookup service creating the DID document JSON-LD file including a suitable keypair, e.g., using the Koblitz Curve, and storing the did.json file under the well-known URL to represent the entire domain.

For example, for the domain name 'support.xck.app', the 'did.json' will be available under the following URL: 'did:web:support.xck.app' -> https://support.xck.app?did.json

Example of the 'did.json' file for 'support.XCK.app'

#### 3.4 Exchange of user profile between the Web and Apps
Did:web users can register their ID in compatible applications, probably from different blockchain networks.  These application will retrieve the user’s profile, validate it by the credentials, facilitating the interaction between them, incrementing the digital capital of these systems. 

A did:web could bring each individual, business or organization a Identity verified web presence, with the capacity to sign, and exchange value in digital networks.

### 4.	Empowering the DID’s with Proof of Identity
Probably, more in the formal space, some legal and business processes, its deliverables, and some cross border transfers, require that the participant users be identified by some valid legal national ID.  DID profiles could be ideal to indicate if there is a valid national identity attribution. Using a technological solution to attribute identity to a DID can be used by each one of these users, authorizing and linking it to the DID, as a proof of identity.  When users are interacting in a transfer or business agreement, this identity attribution could be exchanged between them. This utility of proof of identity could satisfy KYC (Know Your Customer) requirement imposed by some country governments. In this case, regulation, executed in a decentralized way, controlled by each user.

Another complementary Proof of Identity solution could be done by the reference of other users, that they know a certain user.  Kind of a reputation ranking. At a certain, point one or more of the sponsoring users must have a more solid proof of identity issued by a valid legal national ID.  These referrals can also be indicated in the user profile.

### 5.	Storage associated to a BNS name
Apps built with the Stacks blockchain can store off-chain data using a storage system called Gaia.
Gaia is a unique approach to decentralized storage that focuses primarily on user-ownership of data, rather than immutable on-chain storage. In this case the emphasis is on the user control.

While on-chain storage solutions like IPFS and Arweave are designed for immutable, censorship-resistant permanent storage, they cannot be deemed as providing user control of the data since the user cannot modify or remove the data once it has been deployed.

Gaia solves a different problem of allowing users to be in control of where their data is stored while connecting the access of that data to their on-chain Stacks identity.

Whereas public transactional metadata is best stored on the Stacks blockchain, user application data can often be stored more efficiently and privately in Gaia storage.

Storing data off the blockchain ensures that Stacks applications can provide users with high performance and high availability for data reads and writes without introducing central trust parties.

#### a) How GAIA works
When the user logs using its BNS name in to an application, the authentication process gives the application the URL of a Gaia hub, which performs writes on behalf of that user. The Gaia hub authenticates writes to a location by requiring a valid authentication token, generated by a private key authorized to write at that location.

Gaia's approach to decentralization focuses on user-control of data and storage. If a user can choose which Gaia hub and which backend provider to store data with, then that is all the decentralization required to enable user-controlled applications.

#### b) Alternative storage system

The Apps objectives could suggest to use alternative solution to store data associated to a BNS name.  The option of using distributed file system like IPFS, or Arweave, or messaging services like Mastodon, or Matrix, among other type storage services, will be an area of intensive growth in the next years as the decentralization process turns mainstream.  Essentially, these technologies will try bring to market the capacities of the design of Distributed Databases.   

### 6.	Blockchain Inscription service
Immutability is an attribute that Blockchain technology offers to world society.  A transaction, and/or the execution of a smart contract that cannot be alterred.

This attribute of immutability could transformed in an inscription service applied to different purposes.  The first example of this type of service is the BNS, and the second NFT inscriptions for art or music work. Other examples taken from XCK.app are the business agreements inscriptions, payments, and business deliverables inscriptions.  Ordinal inscription is another emerging inscription type.  

Inscriptions could be leverage with the use of did:web for the users, and apps.  An app inscription or an inscription executed by a user could be accessed publicly by a web service using the did:web protocol.  So ideally, blockchain inscriptions could be turned into a standard.  This standard could boost usability among other applications that reference this blockchain inscriptions.

### 7.	DID Domain and subdomain name Exchange of ownership
A market of exchange of DID domain name is already operating.  Since the BNS lets any domain name owner to transfer its property to another user, there has been interest specially among early adopters to save some “key” names for future users, also as the STX exchange value is still low.  There has been some proposal to change the behaviour of the BNS to facilitate storing list of domain names for future exchange.

In the case of DID subdomain names is different, as the list maintained under its DID domain name in the zone file.   Each DID subdomain name owns its own zone file specification, profile file, and its valid hash. The owner of the DID domain name is the only one that can update the list of subdomains under its domain name.   For the exchange of subdomain name between one user to another, the domain name owner must provide a service to transfer its ownership, and executes in behalf of the owner.
 
### 8.	Increasing the BNS or DID utility
Nowadays, the most common use for the blockchain, agreed by several country’s Central Banks, it is its capacity to make cross border assets transfer efficiently.

Lately, the exchange of pieces of art using non fungible tokens, and similarly Ordinals in the Bitcoin network, have attracted the attention generating high level of transaction traffic.

Nevertheless, the use of decentralized ID (DIDs) has not been understood well, and used as it should be.

1.	The use of domain or subdomain names can facilitate the easiness to make inter user token transfer.  
Instead of using the Stacks or Bitcoin addresses, the users can use the DID as the address to execute transactions.
2.	The use of domain or subdomain names can facilitate the easiness to make inter used non fungible token exchange or transfer
Instead of using the Stacks or Bitcoin addresses, the users can use the DID as the address to execute transactions.
3.	Users can use their DID to login into hundreds of available compatible Dapps, like for example in chat boxes, sharing of information, publications, etc.
4.	Users can use their DIDs to login, create and share business process agreements, and deliverables, sign them, and inscribe them in the blockchain using the smart contracts.
5.	Probably, some business process agreements and deliverables, require that the participant users be identified by legal national IDs.  Then a national attribution identity technology can be used by each one of the users, authorizing and linking it to the DID, as a proof of identity.  This utility of proof of identity conforms to the requirement of KYC (Know Your Customer) imposed by some country governments. In this case, regulation, executed in a decentralized way, controlled by each user.
6.	Users can use their did:web definitions as a web presentation landing page presenting their profile information.
7.	Web marketplaces that recognize the use of did:web specification could facilitate the capture of user domain or subdomain names.  These users will not require to re enter profile information, as the did:web specification can be accessed through a .json file and entered to the application.
