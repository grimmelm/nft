# I Do Not Think That NFT Means What You Think It Means #

What do you get when you buy an NFT? The simple answer is "control of a unique
token on a blockchain." But if that's all you get ...

Many NFT owners want something more. When an NFT "comes with" an artwork, they
often expect that the owner of the NFT on the blockchain will also have some
kind of control over the art itself.

You own that piece of art, only you can display it. If you sell the NFT to
someone else, they own the NFT and with it the art. Now only they can display
it.

In addition, some NFTs come with broader rights. For example, Bored Apes say they come with the right to make derivative projects. 
- differentiator from CryptoPunks
- numerous projects in the works, including

This sounds like a new solution to an old issue.

There is only one problem. It doesn't work.

## I Do Not Think That NFT Means What You Think It Means ##

BAYC-style projects are _designed_ to transfer copyrights along with onwership of the NFT itself. They even have [license agreements](t/k) promising to do just that. But these licenses **do not work**. They do not make the copyright licenses travel along with the NFTs the way that they say. If [code is law](t/k), then the Bored Ape license is buggy code.


The idea behind an NFT license is what some lawyers call "tethering": tying ownership of another asset to ownership of the NFT. 

To make this work, two things need to happen. First, whoever _receives_ the NFT on the blockchain also needs to simultaneously receive a copyright license. Second, whoever _transfers_ the NFT also needs to simultaneously _give up_ their license. If either of these steps fails, so does the tethering, because the NFT and the license can becomes severed from each other.

There are some areas of law where transfering one thing also conveys rights to some other thing. One example is a check made out to "cash": whoever (lawfully) has possession of the check is entitled to deposit it. If I give you the piece of paper, I'm also giving you my right to receive payment. The two go together automatically, because the legal system says they do.

But this is _not_ how most areas of law work. If you buy an oil painting from an artist, you do _not_ also receive ownership of the copyright. Yes, you own the original, but the artist retains the copyright, and they can sell prints of it if they like. If you want to buy the copyright too, you'll need to get a signed agreement from them transferring the copyright to you.




The BAYC [Terms & Conditions](https://boredapeyachtclub.com/#/terms) state:

>i. You Own the NFT. Each Bored Ape is an NFT on the Ethereum blockchain. When you purchase an NFT, you own the underlying Bored Ape, the Art, completely. Ownership of the NFT is mediated entirely by the Smart Contract and the Ethereum Network: at no point may we seize, freeze, or otherwise modify the ownership of any Bored Ape.

This looks like it tethers ownership of the copyright to ownership of the NFT. Unfortunately, it doesn't.

First, U.S. copyright law is explicit about what it takes to transfer ownership of a copyright. [Section 204(a)](https://www.law.cornell.edu/uscode/text/17/204) of the Copyright Act states:

>A transfer of copyright ownership, other than by operation of law, is **not valid unless** an instrument of conveyance, or a note or memorandum of the transfer, is **in writing and signed by the owner** of the rights conveyed or such owner’s duly authorized agent. (emphasis added)

The writing part isn't a problem; the terms on the website count as a "writing" under [federal law](https://scholar.google.com/scholar_case?case=7612208998812419954). The bigger issue is that the BAYC terms aren't "signed" by the copyright owner. Without a signature, it is not possible to pass copyright ownership to the holder of the NFT.

This issue is fixable. BAYC's promoters (XXX JG: They _do_ own the copyright in the images they started with, right?) could redo the terms to add a signature line. Under the [E-SIGN Act](https://www.law.cornell.edu/uscode/text/15/7001), even a digital signature like XXX script font signature XXX is enough to constitute a legally valid "signature." Indeed, clicking "I agree" to a website's terms when you create an account [can be a](https://www.law.cornell.edu/uscode/text/15/7006) "process, attached to or logically associated with a contract or other record and executed or adopted by a person with the intent to sign the record." So suppose that this problem is solved, and BAYC successfully transferred copyright ownership in a Bored Ape to the Alice, the first buyer of the NFT. XXX use a specific BA?

The bigger problem comes when Alice decides to resell the Bored Ape to Bob. The intent of the BAYC terms is that Bob now owns the copyright and Alice doesn't. But thanks to the signature requirement, that's not what happens. _There is no signed transfer of copyright from Alice to Bob_. Without a signed transfer, Alice still owns the copyright, not Bob.

Bob might try to argue that Alice has agreed to the BAYC terms, which make him the copyright owner. But Alice hasn't! As far as she's concnered, the BAYC terms are just a bunch of words on a website somewhere. She probably hasn't read them., and she certainly hasn't done anything to agree to them. True, Alice has invoked an ERC-20 smart contract ```transfer()``` method to transfer the Bored Ape to Bob. But that method is a _smart-contract_ term, not a _legal-contract_ term. It doesn't force Alice to agree to anything else. The copyright system wasn't created with ERC-20 tokens in mind and doesn't know about them. As far as it's concerned, Alice owns the Bored Ape copyright and hasn't done anything to give up ownership.

This is not a problem that contract law is well-equipped to solve. Legal contracts typically only bind the people who explicitly agree to them. But since smart contracts exist on the blockchain, it is entrely possible to interact with a smart contract -- for example to transfer and NFT -- without ever invoking any additional contract terms. If copyright in an NFT-linked artwork is based on a legal contract, users who deal only with the smart contract have a decent argument that nothing int he legal contract applies to them, since they interacted with the smart contract.

This is a problem that better-drafted licenses can avoid. One is to use an approach like [RTFKT](https://rtfkt.com/tos), which gives each NFT holder a copyright _license_ rather than copyright _ownership_. That matters because copyright licenses don't need to be signed the way that copyright transfers do. The NFT promoter holds on to the copyright, and simply gives a license directly to each successive holder of the NFT. The details are tricky, but RTFKT at least makes a serious attempt at them. BAYC and the NFT license don't even try. 

Unfortunately, trying to slap a new license on top of an existing one is extremely hard, because if any change reduces the rights that existing NFT holders already have, they can argue that the NFT promoters are trying to give away rights that they no longer have. Only the NFT holders can do so, and they have every right not to. It is far too late for BAYC to change its terms and force all existing Bored Ape owners to agree to them. BAYC can close the yacht club door, but the apes have already left.



