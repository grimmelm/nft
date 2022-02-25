# Copyright Vulnerabilities in NFTs #

Many NFTs and DAOs have run into copyright controversies due to confusion about what 
an NFT actually is and does:

* When the SpiceDAO XXX link bought a copy of the lavishly illustrated pitch
  book that Alejandro Jodorowsky made for a never-filmed version of _Dune_, some
  participants hoped that buying the book would allow them to bring Jodorowsky's
  vision to the screen. But this plan was quickly scrapped when owners of the
  _Dune_ copyrights vetoed the idea.
* "Right-clickers" save JPEG copies of the artwork from popular NFTs. The owners
  of those NFTs say this is copyright infringement. Only one of the two can be
  right.
* XXX more examples

We hope in this blog post to clear up some of the confusion around NFT
copyrights Our bottom line is simple: ownership of an NFT **can** be used to
give the owner substantial control over a creative work, but that control is not
automatic. Copyright law does **not** give an NFT owner any rights unless the
creator takes affirmative steps to make sure that it does. Our survey of some
existing NFT projects and their licenses reveals that **none** of them take all
of the necessary steps needed to make NFT copyrights behave the way that
community members expect. We conclude by describing some potential ways out of
the current mess.

## On-Chain and Off-Chain Assets ##

When talking about blockchain assets, it is common to say things like "Alice
owns 10 Bitcoin." Most of the time, it is clear what this means: Alice controls
the private key to a blockchain address that has been transferred 10 Bitcoin,
and can if she wishes use that private key to transfer those Bitcoin to another
address. (Alice might control the key directly or via a wallet; we will ignore
this complication in what follows.) In the words of the  [current draft Uniform
Commercial
Code](https://www.uniformlaws.org/HigherLogic/System/DownloadDocumentFile.ashx?DocumentFileKey=c7232d9c-6f39-0576-935e-8ad76333240f&forceDialog=0)
article for blockchain assets, Alice has "the power to avail [herself] of
substantially all the benefit from" those Bitcoin. This case is easy because the
Bitcoin are an _on-chain asset_. They exist entirely on the Bitcoin blockchain. 

Matters are more complicated for _off-chain assets_, when an entry on a
blockchain is used to represent an interest in something that exists off the
chain, like a [tungsten
cube](https://opensea.io/assets/0x495f947276749ce646f68ac8c248420045cb7b5e/36033305814565393839012117540795495898903988734891995320738861183142759235585/).
The cube is a physical object. It weights 2,000 pounds, measures 14.545 inches
on a site, and sits in the Willowbrook, Illinois warehouse of Midwest Tungsten
Service (MTS). It exists in the physical world. The Tungsten Cube NFT is an entry in a
smart contract deployed on the Ethereum blockchain using the
[ERC-1155](https://eips.ethereum.org/EIPS/eip-1155) standard. It _refers to_ the
physical cube, but the two are distinct. If Alice buys the tungsten cube NFT
from TungstenDAO, the physical cube will still be sitting in Willowbrook, Illinois.

Althugh the Tungsten Cube NFT is not the _same_ as the physical tungsten cube,
the two are _connected_. According to the "Description" provided by TungstenDAO
to OpenSea when it created the NFT listing, when Alice acquires the NFT, she is
also entitled to "One visit to see/photograph/touch the cube per calendar year."
If she burns the NFT, she is entitled to receive physical possession of the cube
"via freight truck." If she sells the NFT to Bob, then Bob will be entitled to
visit the cube once a year, or to burn the NFT and receive the cube. Some
lawyers call this connectiong "tethering": rights in an off-chain asset (the
physical cube) are linked by an invisible tether to an on-chain asset (the NFT).
(In theory, at least. [Some legal
scholars](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3928901) are
 skeptical about whether tethering actually works.)

Thus, there are actually three diffrent kinds of assets involved in an NFT.
Yes, three.

First, there is an **NFT** itself on the blockchain. It looks like this:

XXX illustration of code / transaction XXX

Second, there is the **physical cube** in a warehouse. It looks like this:

XXX cube picture XXX

Third, there is the **legal right** to control the physical cube. It looks like
this (because legal rights are intangible and have no physical existence:

XXX blank space XXX

If everything works correctly, the legal right is what links the on-chain
NFT to the off-chain cube. The current owner of the NFT is able to
control the physical cube because they _also own_ the associated legal right.

## A Copyright Primer ##

The following quote is sometimes (humorously but incorrectly) [attributed to](https://quoteinvestigator.com/2012/02/24/telegraph-cat/) Albert Einstein:

>You see, wire telegraph is a kind of a very, very long cat.  You pull his tail
>in New York and his head is meowing in Los Angeles.  Do you understand this?
>And radio operates exactly the same way: you send signals here, they receive
>them there.  The only difference is that there is no cat.

A copyright works just like a tungsten cube except that there is no
cube. A tungsten cube is a specific physical object. It exists in one place. Any
other tungsten cube is a different cube. But a creative **work** like a
photograph or a story is intangible. It can exist in many objects (called
**copies**) at once, like when a publisher prints thousands of copies of a book, or when
the photograph is displayed on millions of computer screens. Or it can exist in
no copies at all, like when one person tells another person a story. The point is
that the creative work is not the same as any of the copies that embody it.

Thus, the **copyright** in a creative work behaves differently than ownership
of a physical object, like a tungsten cube. The owher of the cube can move it,
sculpt it, or melt it down; if someone else does any of these, they violate the
owner's property rights. But the owner of a copyright isn't necessarily the owner
of any specific copies. If Alice buys a copy of Bob's novel, Alice owns the
physical copy -- the paper with ink marks on it -- but Bob owns the copyright 
in the words.

Instead, Bob's copyright consists of is a limited set of [exclusive
rights](https://www.law.cornell.edu/uscode/text/17/106). Most importantly, Bob
can prevent anyone, including Alice, from _making more copies_ of his novel.
(That's why it's called a "copy" "right.") If Alice wants to make a movie
adaptation of Bob's novel -- in copyright terminology, a
[derivative](https://www.law.cornell.edu/uscode/text/17/101)
[work](https://www.law.cornell.edu/uscode/text/17/103) -- she needs Bob's
permission. She can get it in one of two ways. Either she can buy the copyright
outright from Bob -- a **transfer** of ownership -- or Bob can retain the
copyright and give Alice a **license** to make the movie. The diffrence is that
if Alice becomes the new owner via transfer, she can now decide whether to
authorize other uses, like graphic novels and action figures. If Bob merely
gives Alice a license, he retains the authority to decide how else to use (or
not) the copyright.

## NFTs, Copies, and Copyrights ##

Back to NFTs. It should be apparent now that an NFT can be tethered to a
creative work in one of two ways. First, it could be used to control a _copy_
of the work: just like whoever owns the Tungsten Cube NFT is entitled to possession
of the tungsten cube, whoever owns the Physical Copy NFT is entitled to posess
a specific copy of the work. Second, it could be used to control the _copyright_
in the work: whoever owns the Intangible Copyright NFT is now entitled to decide
who gets to make new copies. The two could go together, _but they don't have to_.

A number of blockchain projects conflate this distinction. They offer to provide
owners with a copy of a creative work, but _not_ the underlying copyright. XXX
example. This is also where the more grandiose plans for the SpiceDAO went
wrong. Buying a copy of the Jodorowsky book gave its new owners the right to
read it, [sell or lend](https://www.law.cornell.edu/uscode/text/17/109) it to
others, or put it on public display. But it didn't give them the right to make
more copies of the underlying creative works -- the copyrights to which were
still held by the XXX clarify exactly who. 

Another failure mode for NFT copies is that copyright law has an unintuitive
concept of _what counts as a copy_. We have been talking about obviously
distinct physical things, like printed books. But "copies" under [U.S. copyright
law](https://www.law.cornell.edu/uscode/text/17/101) include any "material
objects ... in which a work is fixed by any method now known or later developed,
and from which the work can be perceived, reproduced, or otherwise communicated,
either directly or with the aid of a machine or device." This definition
includes hard drives and SSDs, and sometimes even RAM. Every computer that
interacts with the work makes a separate "copy" for copyright purposes; even
just browsing to a webpage makes a "copy" of the images on it on your computer.
Thus, for all practical purposes any NFT that includes digital artwork _must_
include some copyright interest (either a transfer or a license) or the owner 
of the NFT will become an infringer the moment they attempt to do anything
with the artwork. 

In particular, it is _not_ sufficient to give an NFT purchaser a copy of the
artwork. U.S. copyright law [explicitly
states](https://www.law.cornell.edu/uscode/text/17/202) that transfers of
copyrights and transfers of copies are different:

>Transfer of ownership of any material object, including the copy or phonorecord in which the work is first fixed, does not of itself convey any rights in the copyrighted work embodied in the object; nor, in the absence of an agreement, does transfer of ownership of a copyright or of any exclusive rights under a copyright convey property rights in any material object.

If you buy an oil painting from an artist, you do _not_ also receive ownership
of the copyright. Yes, you own the original, but the artist retains the
copyright, and they can sell prints of it if they like. If you want to buy the
copyright too, you'll need to get a separate agreement. The same is true for
NFTs. Unless an NFT explicitly gives owners _copyright_ interests as opposed to
just access to the artwork, owners should not assume that they have any rights
to use the artwork or to stop others from using it.

We note that some popular NFT projects, including XXX, have been released with
no copyright terms at all. This is legally risky for all concerned. An adversary
could approach the NFT creator, buy out the copyright to the artwork, and then
sue NFT purchasers for infringement if they put the images in their profile
pictures, on OpenSea listngs, etc. This is not the intent of the creators and
purchasers, and we hope that courts would not cooperate in a copyright-based
rugpull like this, but without clarity around the copyright rights of NFT
owners, there is a risk that it could happen. (The courts are not known for
their nuanced understanding of cutting-edge blockchain technologies and
community norms.)

Even more blatantly, an NFT can run afoul of copyright by paying no attention to
it at all. An enormous number of NFT projects are straight-up infringing. They
use artworks stolen from artists, or famous works that the NFT creators have no
connection with and no license from. XXX examples. Copying these works as part
of the NFT marketing (e.g. for OpenSea listings or as downloadable additional
content) can be copyright infringement. In addition, a project that falsely
states or implies that users will receive the legal right to use artworks the
creators have no right to could be engaging in false advertising.

While straight-up scam artists are unlikely to care about infringement, it is
unfortunate that many well-meaning projects also seem to believe that minting an
NFT of a work somehow automatically brings with it some copyright interest in
the work. One particular tragic example is Andy Williams, who [created an
NFT](https://www.washingtonpost.com/technology/2022/02/22/expunge-his-daughters-murder-internet-father-created-an-nft-grisly-video/)
of TV video footage depicting his daughter's murder. Parker was apparently
advised that creating an NFT would give him enough of a copyright in the footage
to have it removed from sites like Facbook and YouTube. But copyright does not
work that way.

## Copyright Transfers Are Hard ##

Actually ensuring that NFT owners have the copyrights they think they do is also 
a subtler problem than it appears. Consider the following passages from the
Bored Ape Yacht Club [Terms & Conditions](https://boredapeyachtclub.com/#/terms):

>i. You Own the NFT. Each Bored Ape is an NFT on the Ethereum blockchain. When
>you purchase an NFT, you own the underlying Bored Ape, the Art, completely.

This looks like it tethers ownership of the copyright to ownership of the NFT.
When Alice buys a Bored Ape NFT, she acquires the copyright. When she sells the
NFT to Bob, he acquires the copyright. In copyright terms, there is a transfer
of copyright ownership to Alice when she buys the NFT, and then another one from
Alice to Bob when she sells him the NFT. Full ownership of the copyright lets
Alice use the artwork -- e.g. to display in her Twitter profile inside a
hexagon. It also lets her sue for infringement, if she wishes, any
right-clickers who download and display the artwork.

XXX Diagram:
Yuga Labs -> Alice -> Bob

Unfortunately, _copyright doesn't work this way_. The problem is that U.S.
copyright law sets a high threshold for what it takes to transfer ownership of a
copyright. [Section 204(a)](https://www.law.cornell.edu/uscode/text/17/204) of
the Copyright Act states:

>A transfer of copyright ownership, other than by operation of law, is **not
>valid unless** an instrument of conveyance, or a note or memorandum of the
>transfer, is **in writing and signed by the owner** of the rights conveyed or
>such owner’s duly authorized agent. (emphasis added)

The writing part isn't a problem; the terms on the website count as a "writing"
under [federal
law](https://scholar.google.com/scholar_case?case=7612208998812419954). The
bigger issue is that the BAYC terms aren't "signed" by the copyright owner, Yuga
Labs. Without a signature, it is not possible to pass ownership of the copyright to Alice.

In theory, Yuga Labs could fix the lack of a signature at this first step by
redoing the BAYC terms to add a signature line. Under the [E-SIGN
Act](https://www.law.cornell.edu/uscode/text/15/7001), even a digital signature
like XXX script font signature XXX is enough to constitute a legally valid
"signature." Indeed, clicking "I agree" to a website's terms when you create an
account [can be a](https://www.law.cornell.edu/uscode/text/15/7006) "process,
attached to or logically associated with a contract or other record and executed
or adopted by a person with the intent to sign the record." There is a bit of
timing issue, in that Alice owns the NFT now, so changing the terms going
forward would work for any future sales but wouldn't retroactively cover the
initial sale to Alice. But Yuga Labs could execute a special one-time transfer
to the current owners of all of its Bored Apes.

Unfortunately, there is a bigger problem. It arises when Alice decides to resell
the Bored Ape to Bob. The intent of the BAYC terms is that Bob now owns the
copyright and Alice doesn't. But thanks to the signature requirement, that's not
what happens. _There is no signed transfer of copyright from Alice to Bob_.
Without a signed transfer, Alice still owns the copyright, not Bob.

Bob might try to argue that Alice has agreed to the BAYC terms, which make him
the copyright owner. But Alice hasn't! As far as she's concnered, the BAYC terms
are just a bunch of words on a website somewhere. She probably hasn't read
them, and she certainly hasn't done anything to agree to them. True, Alice has
invoked an ERC-20 smart contract ```transfer()``` method to transfer the Bored
Ape to Bob. But that method is a _smart-contract_ term, not a _legal-contract_
term. It doesn't force Alice to agree to anything else. The copyright system
wasn't created with ERC-20 tokens in mind and doesn't know about them. As far as
it's concerned, Alice owns the Bored Ape copyright and hasn't done anything to
give up ownership.

This is not a problem that contract law is well-equipped to solve. Legal
contracts typically only bind the people who explicitly agree to them. But since
smart contracts exist on the blockchain, it is entrely possible to interact with
a smart contract -- for example to transfer and NFT -- without ever invoking any
additional contract terms. If copyright in an NFT-linked artwork is based on a
legal contract, users who deal only with the smart contract have a decent
argument that nothing in the legal contract applies to them, since they
interacted with the smart contract.

## An Alternative: Copyright Licenses ##

There is another way to structure NFT copyrights that avoids the signed-writing
problem. Instead of a _transfer of ownership_, which passes full copyright
ownership to each owner of the NFT, the NFT creator could use a _copyright license_. 
The creator holds on to ownership of the copyright, and gives a license directly
to each successive NFT owner.

Woodchuck Labs
|             |         |
|             |         |
Alice   ->   Bob ->    Carol

At first glance, this looks more complicated, because now the creator must deal
directly with every NFT owner, rather than just with the first owner. But it has
a subjstantial advantage, which is that copyright licenses don't need to be
signed the way that copyright transfers do.  (Indeed, they don't even need to be
[in writing](https://scholar.google.com/scholar_case?case=9695307318571874997),
although for any economically serious transactions, writing down the terms is
mush safer.) Carol and Woodchuck Labs don't need to rely on Alice and Bob to get
the signed-transfers right. Instead, Woodchuck Labs can simply write its terms
so that it directly gives a license to every NFT owner _automatically_ as soon
as they acquire the NFT.

There are good precedents for this approach in free and open-source software
licensing. The GNU [General Public
License](https://www.gnu.org/licenses/gpl-3.0.en.html), for example, says:

>Each time you convey a covered work, the recipient **automatically receives a
license** from the original licensors, to run, modify and propagate that work,
subject to this License. You are not responsible for enforcing compliance by
third parties with this License.

And the [Creative Commons Attribution
license](https://creativecommons.org/licenses/by/4.0/legalcode) says:

>Every recipient of the Licensed Material **automatically receives** an offer
from the Licensor to exercise the Licensed Rights under the terms and
conditions of this Public License.

A clear example of this aproach in the NFT space is the
[RTFKT](https://rtfkt.com/tos) license, which states:

>1 ... Any digital works of authorship or other content made available through
>the Platform to an owner of a Digital Collectible that is intended as an
>“Additional Benefit” (as that term is defined in the Digital Collectible Terms)
>will be identified as such on the Platform or at the time of download. **Any
>such content will be licensed to you for as long as you own the applicable
>Digital Collectible** pursuant to the terms of any license presented at the
>time of download or, if no such terms are presented, pursuant to the applicable
>Digital Collectible Terms as Related Content for that particular Digital
>Collectible.  ...

The details are tricky, and this is not meant to be a full legal analysis. Our
points are just that NFT creators need to give serious thought to how they
structure their terms to ensure that NFT owners actually receive the necessary
copyright licenses to NFT-linked artwork, and that copyright licensing is far
easier to make work than an outright transfer of ownership.


## Derivative Rights ##

Another difficult issue concerns derivative works -- i.e., "a translation,
musical arrangement, dramatization, fictionalization, motion picture version,
sound recording, art reproduction, abridgment, condensation, or **any other form
in which a work may be recast, transformed, or adapted**." No one can explain
why the Bored Apes achieved cultural and economic escape velocity. It will
forever be one of the mysteries of the ages. But one factor, at least, is
sometimes [said to
be](https://thedefiant.io/bored-apes-yacht-club-cryptopunks-copyright-fight/)
that the Bored Apes terms allow owners to make more extensive derivative works
based on them. While the [NFT license](https://www.nftlicense.org) allows
owners to use the art for their own "personal, non-commercial use" and for
projects earning up to $100,000 per year, the BAYC terms allow unrestricted
commercial use of the artworks. Specifically, "Yuga Labs LLC grants you an unlimited,
worldwide license to use, copy, and display the purchased Art for the purpose of
creating derivative works based upon the Art."

The first problem here is that this license grant is inconsistent with the
statement, just two paragraphs above in the BAYC terms, that "[w]hen you
purchase an NFT, **you own the underlying Bored Ape, the Art, completely**." If
Alice really does "own" the art "completely," then Yuga Labs has nothing left to
give and the commercial-use license is superflous. (This is another sign that
the statement that Bored Ape NFT owners "own" the artwork, like many other
claims about [what users actually
own](https://scholarship.law.upenn.edu/penn_law_review/vol165/iss2/2/) when they
"buy" content online, cannot be taken at face value.)

The second problem is that this term does not play nicely with downstream
transfers. Suppose that Alice owns Bored Ape NFT number 12345. She allows Fern,
a a filmmaker, to create a video series based on Bored Ape 12345. Those videos
are derivative works under copyright law and Fern  has their own copyright in
the videos. Now Alice decides to sell Ape number 12345 to Bob. _What should
happen to Fern's license?_

Yuga Labs
|
|
Alice -> Bob
|
|
Fern

One simple answer would be that since Alice's copyright license to use Bored Ape
12345 terminates when her ownership of the NFT does, so do any sublicenses she
has granted. That would mean that the videos stop being licensed the moment
Alice sells to Bob, and Fern becomes a copyright infringer if they continue to
show the videos! This is terrible from Fern's perspective, having invested time
and money into making the videos. It's also terrible from Alice's perspective,
because Fern ought to be very reluctant to pay money to license Alice's rights
if Alice can always rugpull by selling the NFT to Bob. So this solution
effectively makes the derivative work rights unmarketable.

Yuga Labs
|
|
Alice -> Bob
|
X
|
Fern

Another answer would be that Fern's license continues in full force. Bob has no
ability to call backsies once Alice has given Fern a license. This protects
Fern, and thereby protects Alice's licensing business. But it creates its own
headaches. For example, Bob might grant his own video license to Georg, so now
there are two competing Bored Ape 12345 series. Fern will be furious, but what
can they do about it? If their lawyers are good, Fern will have insisted that
Alice make the video license exclusive, so that Alice can no longer license
anyone else to make a video series. But this is a private contract between Alice
and Fern. Bob didn't sign it, and isn't bound by it! Bob got his copyright
license direct from Yuga Labs, without the exclusivity limitation that Alice
promised to Fern.

So maybe the licenses ought to travel with the NFT itself. This happens all the
time with real estate. If Alice owns a parcel of land and grants Telecorp an
"easement" to run a fiber-optic cable under one corner of her land, the easement
will still exist after Alice sells the land to Bob. It is said to "bind the
owner's sucessors" or to "run with the land." That is the easement is attached
to and limits (or "burdens") the legal right to the land itself. It is not just
a personal promise from Alice to Telecorp. When Bob buys the land from Alice, he
steps into her shoes. He succeeds not just to her rights in the land (e.g. to
build a house or grow crops), but also to her obligations (to allow Telecorp to
continue to operate the cable).

Alice -> Bob
|        |
|        |
Telecorp

Similarly, we could imagine that when Bob buys the NFT from Alice, he steps into
her shoes. He succeeds not just to Alice's rights in the Bored Ape 12345
copyright (such as the right to make glossy art prints), but also to any
limitations or obligations Alice has taken on (such as the exclusive video
license to Fern). Now Bob is not free to to license Georg to make a second video
series.

Alice -> Bob
|        |
|        |
Fern

Perhaps this is a good solution. Or perhaps not. If Alice is now free to
encumber the artwork copyright in this way, it limits Bob's rights. When he buys
the NFT, he buys something less than the full rights Alice bought. Alice has
carved up the copyright, and in effect kept a slice for herself. If Bob is in
the NFT market, he will have to investigate the entire chain of title of the NFT
he is buying to make sure that no Alices before him have quietly given away part
of the copyright. This need for investigation runs contrary to the crypto ethos
that as much as possible should be don in public and on-chain. So maybe exclusive
licenses entered into by one owner should _not_ run with the NFT.

So far, we have enumerated three different possibilities for what happens when
Alice sells the NFT to Bob:

1. Fern's license terminates.
2. Fern's license continues, but Bob can license the same rights to Georg.
3. Fern's license continues, and Bob cannot license the same rights to Georg.
   
It is possible to imagine a court adopting any of these three outcomes. Indeed,
there is no clear consensus as to which of these is the best solution in
general. (The three of us don't even agree!) Even worse, these don't even
exhaust the possibilities. A fourth possibility is that Fern's license to create
_new_ derivative works terminates, but that they can continue to use _existing_
derivative works they have already created. This is how copyright law [deals
with](https://scholar.google.com/scholar_case?case=6610856779804662857) some
license terminations, including most famously the film rights to _Rear Window_.
Or if Fern's license continues, what should happen to any royalties that Fern
has promised to pay Alice? Should Bob suceed to those too? There are arguments
in favor, and arguments against.

Our point is just that **these are issues that an NFT license allowing
derivative works needs to deal with**. Otherwise, NFT owners and their business
partners may be unpleasantly surprised by the results. Everyone who does a
project based on an NFT that does not answer these questions is putting an
immense amount of faith in the courts to get things right if the deal goes sour
and the parties end up suing each other.

We are not saying that there is a best solution for all projects. (This is one
reason among many that we are not proviidng our own proposed license text.) What
is right for the Bored Apes may not be right for an NFT project based aroud
musical works, or on a literary work. Instead, we think that NFT creators need
to think about these issues, discuss them with their communities, and then
communicate clearly how copyright licenses will work in relation to the NFTs.



## Conclusion ##

It is clear that many NFT projects are  _designed_ to transfer copyrights along
with onwership of the NFT itself. This is a core design goal, on the same level
as creating compelling content and making transfers irrevocable. Despite this,
many projects seem to have put far less thought into the legal aspects of their
designs than into the technical and artistic ones.

We think this is a major mistake. The legal infrastructure on which blockchains
run is just as complicated and full of traps for the unwary as the technical
infrastructure. While some cryptocurrency and web3 projects are intended to
escape the existing legal system, or to replace it entirely, the same is not
true of many creative NFT projects. They are intended to work within the legal
system as it currently exists, to allow people to create new and interesting art
_now_, and to commercialize it using real-world contract, property, and
copyright law.

Many existing NFT licenses are not fit for purpose. They do not make copyright
interests travel along with the NFTs in the way that they intend. If [code is
law](t/k), then these licenses are buggy code. Responsible NFT creators would
not launch a project built atop a smart-contract library that had known
unpatched vulnerabilities. They should bring the same care to the legal code
on which they depend, because otherwise the results could be just as catastrophic.
