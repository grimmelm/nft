# The IC3 NFT License

The IC3 License links an NFT with a copyright license to use a creative work. The license travels with ownership of the NFT, so that when the NFT is transferred, so is the license. 

## Introduction

The IC3 License has been specifically designed to work with blockchain-based NFTs, e.g. with smart contracts that implement the standard defined in [EIP-721](https://eips.ethereum.org/EIPS/eip-721). But it is not restricted to blockchain-based NFTs. The license uses the technology-neutral term "Ledger" to refer to the system that records information about NFTs and their owners. The license can be used with any underlying technology as long as it (1) supports persistent unique identifiers to serve as NFTs, (2) associates those NFTs with specific owners, (3) allows the owner of an NFT to control the it with a cryptographic key, and (4) allows an NFT to be linked to a creative work. This system can be widely distributed (like a public blockchain), moderately distributed (like a private blockchain), or fully centralized (like a database with a single administrator). Use of the IC3 License for other kinds of licensing is strongly discouraged.

The IC3 License has also been specifically designed to work with NFTs that implement the interface defined in EIP-XXX. This is a general smart contract interface that provides modular support for common features in copyright licensing, including transfer, sublicensing, and revocation. The IC3 License can also be used with NFTs that implement the generic NFT interface defined in EIP-721, or with other NFTs, but the EIP-XXX interface is recommended to reduce ambiguity about when there has been a transfer, sublicense, or revocation.


## Taking Effect

The IC3 License is structured as a license, rather than a contract. The licensor unilaterally grants a copyright license to the current owner of the NFT. The owner does not need to do anything to accept the license; they receive it automatically. If the owner transfers the NFT to someone else, the license transfers with them. The previous owner is no longer licensed; the new owner receives a license on exactly the same terms. This too is automatic, the new owner does not need to do anything to accept the license.

Standard techniques used by lawyers to create binding terms of use for websites do not work for NFTs on blockchains. Consider the clickthrough agreements used by websites: when you create an account, you must check a box indicating that you agree to the website's terms of use. This works because you have taken an action (checking the box) that is clearly and specifically linked to the legal terms and nothing else. There is no question about whether you meant to agree when you checked the box, because there is no other reason to check the box. 

But a blockchain does not have a checkbox or even a website. Someone who receives an EIP-721 NFT need not have done anything at all. They may never have visited the NFT sponsor's website, or even know about this. This means that any promises by the _licensee_ in a license contract are  illusory. Licensor has no guarantee that a downstream NFT owner has actually agreed to the license terms. Thus, the IC3 License does not give the licensee any duties, so there is no need for them to agree to anything.

On the other hand, the IC3 License does attempt to ensure that the _licensor_ has clearly indicated their intent to be bound by the license terms. It does so by saying that the license becomes effective when the licensor "Invokes" it through a "Licensing Process," i.e., uses a technical process to connect an NFT with the IC3 License. This definition includes (but is not limited to) the EIP-XXX interface. 

The essential idea of  EIP-XXX  is to make it explicit when a licensor intends to create a copyright license. Any smart contract that has effects _other_ than creating a license runs the risk that courts might hold that the licensor activated it for those other effects, rather than to create a license. By removing all such other effects, the EIP-XXX interface strengthens the inference that the licensor specifically intended to create a license. (If you do not want to create a license, do not invoke an EIP-XXX method.)


## License Terms

The actual license grant is the least important part of the IC3 License! We have tried to capture the most common and important use cases in light of the NFT community's responses to previous licenses. But our goal has been simplicity rather than perfection. If you want to tweak the IC3 License to meet your own needs, this is the part to tinker with.

Drawing on the success of the Creative Commons license suite, the IC3 License can be customized to be either Commercial or NonCommercial (C vs. NC), and to allow Derivative works or to specify No Derivative works (D vs. ND). These two options can be set independently, for a total of four variations. We did not include a Creative Commons-style ShareAlike option for derivative works. A licensor who is interested in establishing a shared pool of creative works should use an open license that lets anyone make derivative works (such as the CC BY-SA license or the GPL), rather than a license tied to an NFT.

The IC3 License applies to "Licensed Material" that is "Linked" to an NFT. The definition of Licensed Material is deliberately broad: it can include highly creative works like images or videos, but it also includes "other material" to include datasets, software, or other works that are not primarily artistic. The definition of Linked is also broad: it can be by hyperlink, by description, or through a hash value. What is important is that the NFT must be connected to specific licensed material in a way that cannot change over time. We do not attempt to solve the (very difficult) problems of creating a technical standard or a license for an NFT whose contents can change over time.

The core license grant in the IC3 License is that the owner can "Use" the licensed material, i.e. exercise all of the usual rights under copyright to make copies of the work and share them with the public. This is an unlimited grant: it covers all media, digital and analog, on-chain and off-chain. If the license is NonCommercial, it excludes any uses directed to "commercial advantage or monetary compensation," which includes any cases in which people are required to pay to get a copy of the work. Whether the license is Commercial or NonCommercial, no royalties are required.

If the licensor chooses to allow derivative works, then the license grant also allows the owner to use "Adapted Material," which uses language from the Creative Commons license suite to define what counts as a derivative work. To reflect the customs of the NFT community, we added langauge to make clear that simply reproducing the work in a different medium -- e.g., printing T-shirts of a JPEG -- doesn't count as making a derivative work. Only new projects -- such as modifying artwork, remixing a song, or making a TV series based on a character -- are derivative works.

Regardless of which license option is used, all versions of the IC3 License include two specific uses that are always allowed. First, the material can be used to sell the NFT, e.g. on an OpenSea listing. This is an essential part of truth in advertising; someone considering buying the NFT typically needs to be able to see what creative work they will actually be getting. A similar clause is present in many other NFT licenses, although we have attempted to generalize it so that it is less tied to the specifics of how any particular NFT marketplace works. Second, the IC3 License generally allows free use of the material to identify the owner publicly, e.g. in a Twitter profile hexagon. This too is widespread in the NFT community and widely allowed by other NFT licenses.


## Transfer, Revocation, and Sublicensing

The IC3 License tries to deal sensibly with the many complications that can arise due to the free transferability of NFTs. Most existing NFT licenses have not taken this possibility seriously, even though it is arguably _the_ defining characteristic of NFTs and the one that makes them most appealing to users.

The first major issue is that NFTs can be, and frequently are, stolen. A hacker or phisher gains access to an NFT owner's private key and uses it to transfer the NFT to themself, frequently turning around and immediately reselling it. Under these circumstances, should the _copyright_ license stay with the previous owner of the NFT, or go to the new owner? There are at least three possible answers a license could take:

1. The license follows the NFT. The old owner's license terminates, and the new owner receives a license. This approach makes the blockchain reliable and authoritative, but it also makes it difficult for NFT owners to commercialize derivative works of their NFTs unless they take extreme security measures.
2. The license stays with the true owner of the NFT according to property law. This approach makes the blockchain non-authoritative and can require additional investigation on the part of buyers and licensees, but it protects NFT owners against theft, fraud, and duress.
3. The license defines its own rules and specifies the circumstances under which it does and does not transfer. This approach allows for fine-tuning, but at the cost of incompatibility with both the blockchain and with the legal system.

The IC3 license follows option (2). Our reasoning is that the choice to use a copyright license at all indicates that integration with the existing legal system is an essential goal. The license therefore defers entirely to "the property laws of the relevant jurisdiction" in determining who qualifies as the owner of an NFT. To keep the distinction clear, it uses the term "Controller" for the person who has control of an NFT via a private key, and "Owner" for the person who is legally entitled to control it, whether they actually do or not. Thus, the IC3 license defines the "Transfer" of an NFT in terms of a change in who is the Owner of the NFT, not in terms of who is its Controller.

The IC3 License can be revoked, but it does not define the conditions under which it can be. This may seem paradoxical, but it reflects the design goal of making the license itself simple and modular. Instead, the license _defers_ to the smart contract that invoked it in the first place. If that contract says that the license has been revoked, it has been. The EIP-XXX interface defines a generic revocation function, which the parties can plug into any smart contract they want to define the conditions under which the license terminates. That could be the simple passage of time, the unilateral choice of one of them, more complicated logic, or nothing. The point is that all of these options are equally compatible with the core license grant of the IC3 License, and thus they can all be outside its scope. Once again, the license is designed to work with the EIP-XXX interface, but it is drafted so that any technical process serving the same function can be used instead.

The IC3 License takes a similarly broad and deferential attitude toward sublicensing. In practice, sublicensing is likely to be particularly useful in two scenarios. First, the owner may wish to contract with others to produce goods embodying the work, like T-shirts or song downloads. Here, a sublicense is practically necessary in a world where people don't personally print T-shirts and host downloads, but instead hire professionals to do it for them. Second, sublicensing is necessary for many derivative works: producing an animated video series, for example, will require a sublicense to a production company. Thus, the license generally allows for the free sublicensing of any of the rights held by the NFT owner.

As with revocation, the IC3 License allows for a sublicense to be recorded on the blockchain, and as with revocation, these sublicenses are specifically supported by EIP-XXX. Again, the support is generic; the sublicense must include a link to its terms, and EIP-XXX does not attempt to verify that the sublicense's terms are compatible with the license's terms. Indeed, the license does _not_ require that all sublicenses be explicitly recorded in the smart contract; for a T-shirt vendor or a web host, this is overkill. 

Instead, the advantage of recording a sublicense on the blockchain is that it makes the sublicense transfer with the NFT. The IC3 License provides that all sublicenses that have been recorded this way carry over and remain as sublicenses from the new owner of the NFT. Someone who wants to make a substantial investment in an NFT -- e.g., a filmmaker creating a movie based on an NFT-licensed work -- can record this license in the EIP-XXX smart contract. This puts everyone in the world (including potential buyers of the NFT) on notice of their sublicense and that it will carry over. (This is similar to how recording systems for copyrights and real property work, and the EIP-XXX interface has been designed to make this notice straightforward.)   


## Interpretation

The IC3 License concludes with a section advising courts on how to interpret it in the event of a dispute. Although the license itself does not force the copyright license to keep in sync with ownership on the blockchain, it advises courts that maintaining the reliability of blockchain records is an important goal, encouraging them to pick interpretations that make the blockchain a useful and authoritative source for understanding the status of a copyright license. In addition, the interpretation clause encourages courts to promote other common legal policies, such as fairness, uniformity, and predictability.