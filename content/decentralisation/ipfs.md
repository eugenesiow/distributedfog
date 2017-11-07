---
title: "IPFS"
full: "InterPlanetary File System"
type: "article"
description: "InterPlanetary File System (IPFS) is a protocol designed to create a permanent and decentralized method of storing and sharing files. It is a content-addressable, peer-to-peer hypermedia distribution protocol. Nodes in the IPFS network form a distributed file system."
tags: ["software","decentralised","distributed","merkle"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### IPNS
IPFS has a name service called IPNS, a global namespace based on PKI, serves to build trust chains, is compatible with other NSes and can map DNS, .onion, .bit, etc. to IPNS. It is a way to add a small amount of mutability to the permanent immutability that is IPFS. It allows you to store a reference to an IPFS hash under the namespace of your peerID (the hash of your public key).
{{% /card %}}

{{% card size="4" %}}
### Quick Summary [...](https://github.com/ipfs/ipfs/blob/master/README.md#who-designed-it)
- IPFS is a protocol
- IPFS is a filesystem
- IPFS is a web
- IPFS is modular
- IPFS uses crypto
- IPFS is P2P
- IPFS is a CDN
{{% /card %}}

{{% card size="8" small="IPFS whitepaper" %}}
The InterPlanetary File System (IPFS) is a peer-to-peer distributed file system that seeks to connect all computing devices with the same system of files. In some ways, IPFS
is similar to the Web, but IPFS could be seen as a single BitTorrent swarm, exchanging objects within one Git repository. In other words, IPFS provides a high throughput content-addressed block storage model, with content addressed hyperlinks. This forms a generalized Merkle DAG, a data structure upon which one can build versioned file systems, blockchains, and even a Permanent Web. IPFS combines a distributed hashtable, an incentivized block exchange, and a self-certifying namespace. IPFS has no single point of failure, and nodes do not need to trust each other.

##### How IPFS works?
- Each file and all of the blocks within it are given a unique fingerprint called a cryptographic hash.
- IPFS removes duplications across the network and tracks version history for every file.
- Each network node stores only content it is interested in, and some indexing information that helps figure out who is storing what.
- When looking up files, you're asking the network to find nodes storing the content behind a unique hash.
- Every file can be found by human-readable names using a decentralized naming system called IPNS.
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://ipfs.io/" "IPFS Site">}}
    {{<listlink "https://ipfs.io/docs/" "IPFS Documentation">}}
    {{<listlink "https://discuss.ipfs.io/" "IPFS Community">}}
    {{<listlink "https://github.com/ipfs/papers/raw/master/ipfs-cap2pfs/ipfs-p2p-file-system.pdf" "IPFS Whitepaper">}}    
{{< /listcard >}}