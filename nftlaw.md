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



## Doing It Wrong: Bored Apes ##


The BAYC [Terms & Conditions](https://boredapeyachtclub.com/#/terms) state:

>i. You Own the NFT. Each Bored Ape is an NFT on the Ethereum blockchain. When you purchase an NFT, you own the underlying Bored Ape, the Art, completely. Ownership of the NFT is mediated entirely by the Smart Contract and the Ethereum Network: at no point may we seize, freeze, or otherwise modify the ownership of any Bored Ape.

This looks like it tethers ownership of the copyright to ownership of the NFT. Unfortunately, it doesn't.

First, U.S. copyright law is explicit about what it takes to transfer ownership of a copyright. [Section 204(a)](https://www.law.cornell.edu/uscode/text/17/204) of the Copyright Act states:

>A transfer of copyright ownership, other than by operation of law, is **not valid unless** an instrument of conveyance, or a note or memorandum of the transfer, is **in writing and signed by the owner** of the rights conveyed or such owner’s duly authorized agent. (emphasis added)

The writing part isn't a problem; the terms on the website count as a "writing" under [federal law](https://scholar.google.com/scholar_case?case=7612208998812419954). The bigger issue is that the BAYC terms aren't "signed" by the copyright owner. Without a signature, it is not possible to pass copyright ownership to the holder of the NFT.

This issue is fixable. BAYC's promoters (XXX JG: They _do_ own the copyright in the images they started with, right?) could redo the terms to add a signature line. Under the [E-SIGN Act](https://www.law.cornell.edu/uscode/text/15/7001), even a digital signature like XXX script font signature XXX is enough to constitute a legally valid "signature." Indeed, clicking "I agree" to a website's terms when you create an account [can be a](https://www.law.cornell.edu/uscode/text/15/7006) "process, attached to or logically associated with a contract or other record and executed or adopted by a person with the intent to sign the record." So suppose that this problem is solved, and BAYC successfully transferred copyright ownership in a Bored Ape to the Alice, the first buyer of the NFT. XXX use a specific BA?

The bigger problem comes when Alice decides to resell the Bored Ape to Bob. The intent of the BAYC terms is that Bob now owns the copyright and Alice doesn't. But thanks to the signature requirement, that's not what happens. _There is no signed transfer of copyright from Alice to Bob_. Without a signed transfer, Alice still owns the copyright, not Bob.

Bob might try to argue that Alice has agreed to the BAYC terms, which make him the copyright owner. But Alice hasn't! As far as she's concnered, the BAYC terms are just a bunch of words on a website somewhere. She probably hasn't read them., and she certainly hasn't done anything to agree to them. True, Alice has invoked an ERC-20 smart contract ```transfer()``` method to transfer the Bored Ape to Bob. But that method is a _smart-contract_ term, not a _legal-contract_ term. It doesn't force Alice to agree to anything else. The copyright system wasn't created with ERC-20 tokens in mind and doesn't know about them. As far as it's concerned, Alice owns the Bored Ape copyright and hasn't done anything to give up ownership.

This is not a problem that contract law is well-equipped to solve. Legal contracts typically only bind the people who explicitly agree to them. But since smart contracts exist on the blockchain, it is entrely possible to interact with a smart contract -- for example to transfer and NFT -- without ever invoking any additional contract terms. If copyright in an NFT-linked artwork is based on a legal contract, users who deal only with the smart contract have a decent argument that nothing in the legal contract applies to them, since they interacted with the smart contract.

## Doing It Right: RTFKT ##

This is a problem that better-drafted licenses can avoid. One is to use an approach like [RTFKT](https://rtfkt.com/tos), which gives each NFT holder a copyright _license_ rather than copyright _ownership_. That matters because copyright licenses don't need to be signed the way that copyright transfers do. The NFT promoter holds on to the copyright, and simply gives a license directly to each successive holder of the NFT.  Here is the relevant language from the RTFKT terms:

>1 ... Any digital works of authorship or other content made available through the Platform to an owner of a Digital Collectible that is intended as an “Additional Benefit” (as that term is defined in the Digital Collectible Terms) will be identified as such on the Platform or at the time of download. **Any such content will be licensed to you for as long as you own the applicable Digital Collectible** pursuant to the terms of any license presented at the time of download or, if no such terms are presented, pursuant to the applicable Digital Collectible Terms as Related Content for that particular Digital Collectible.  ...

The details are tricky, and the RTFKT approach does not necessarily get all of them right in all cases. But at least it makes a serious attempt at the problem. BAYC and the NFT license don't even try. 

Unfortunately, now that the Bored Apes (and other NFTs using similar licenses) are loose on the blockchain, trying to relicense them is extremely hard, perhaps impossible. An open-source developer can always release their software under a new and more permissive license; they are just giving more rights to users around the world. But because the crucial feature of an NFT license is that it doesn't just _give_ rights to transferees but _takes away_ rights from transferrors, changing the license terms typically means tring to limit the rights of existing NFT owners. Those owners can argue, quite persuasively, that those rights can't be taken away without their permission. It is far too late for BAYC to change its terms and force all existing Bored Ape owners to agree to them. BAYC can close the yacht club door, but the apes have already left.


## Derivative Rights ##

No one can explain why the Bored Apes achieved cultural and economic escape velocity. It will forever be one of the mysteries of the ages. But one factor, at least, is sometimes [said to be](https://thedefiant.io/bored-apes-yacht-club-cryptopunks-copyright-fight/) that the Bored Apes terms allow owners to make more extensive use of them. While the base [NFT license](https://www.nftlicense.org) allows owners to use the art for their own "personal, non-commercial use" and for projects earning up to $100,000 per year, the BAYC terms allow unrestricted commercial use of the art. Specifically, "Yuga Labs LLC grants you an unlimited, worldwide license to use, copy, and display the purchased Art for the purpose of creating derivative works based upon the Art."

The first problem here is that this license grant is completely inconsistent with the statement, just two paragraphs above in the BAYC terms, that "[w]hen you purchase an NFT, **you own the underlying Bored Ape, the Art, completely**." If Alice really does "own" the art "completely," then Yuga Labs has nothing left to give and the commercial-use license is superflous. (This is another sign that the statement that Bored Ape NFT owners "own" the artwork cannot be taken at face value. Whether this means that Yuga Labs or other Bored Ape promoters have engaged in securities fraud or false advertising by misdescribing the rights that come along with NFT ownership is a question best left for another day.)

The second problem is that this term, too, does not seem to have been written with the possibility of NFT transfers in mind, **even though free transferrability on the blockchain is one of the defining features of NFTs**. Suppose that Alice owns Bored Ape NFT number 12345. She allows Fern, a a filmmaker, to create a video series based on Bored Ape 12345. Those videos are "[derivative](https://www.law.cornell.edu/uscode/text/17/101) [works](https://www.law.cornell.edu/uscode/text/17/103)" under copyright law and Fern  has their own copyright in the videos. Now Alice decides to sell Ape number 12345 to Bob. _What should happen to Fern's license?_

One simple answer would be that since Alice's copyright license to use Bored Ape 12345 terminates when her ownership of the NFT does, so do any sublicenses she has granted. That would mean that the videos stop being licensed the moment Alice sells to Bob, and Fern becomes a copyright infringer if they continue to show the videos! This is terrible from Fern's perspective, having invested time and money into making the videos. It's also terrible from Alice's perspective, because Fern ought to be very reluctant to pay money to license Alice's rights if Alice can always rugpull by selling the NFT to Bob. So this solution effectively makes the derivative work rights unmarketable.

Another answer would that Fern's license continues in full force. Bob has no ability to call backsies once Alice has given Fern a license. This protects Fern, and thereby protects Alice's licensing business. But it creates its own headaches. For example, Bob might grant his own video license to Georg, so now there are two competing Bored Ape 12345 series. Fern will be furious, but what can they do about it? If their lawyers are good, Fern will have insisted that Alice make the video license exclusive, so that Alice can no longer license anyone else to make a video series. But this is a private contract between Alice and Fern. Bob didn't sign it, and isn't bound by it! Bob got his copyright license direct from Yuga Labs, without the exclusivity limitation that Alice promised to Fern.

So maybe the licenses ought to travel with the NFT itself. When Bob buys the NFT from Alice, he steps into her shoes. He succeeds not just to Alice's rights in the Bored Ape 12345 copyright (such as the right to make glossy art prints), but also to any limitations or obligations Alice has taken on (such as the exclusive video license to Fern). Now Bob is not free to to license Georg to make a second video series.

Problem solved? Perhaps. Complications remain -- for example, what should happen to any royalties that Fern has promised to pay Alice? Should Bob suceed to those too? There are arguments in favor, and arguments against. Our point is just that **these are issues a serious NFT copyright license needs to deal with**. Despite this, the BAYC, NFT, and RTFKT licenses are _completely silent_ on the subject. Everyone who does a project based on an NFT using one of these licenses is putting an immense amount of faith in the courts to get things right if the deal goes sour and Alice, Bob, Fern, and Georg end up suing each other.