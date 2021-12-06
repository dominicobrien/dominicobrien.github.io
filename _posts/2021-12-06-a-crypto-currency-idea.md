---
title: "A Crypto Currency Idea"
date: 2021-12-06T14:14:05+01:00
categories:
  - Politics
tags:
  - Money
  - Finance
  - Finanial Reform
---
Did you ever read my 2019 paper on money? Because this crypto currency idea is based around that. I think it would be quite a revolution if it could be implemented.
You can find it here: "[The Reason Behind Financial Crisis]({% post_url 2019-09-15-the-reason-behind-financial-crisis %})".

But I can explain quickly in a nutshell so you don't have to go and read that first:

Basically banks create money by issuing loans, I am not sure you are aware but that is where all of our money is currently coming from. There is no other mechanism today other than issuing a loan is = making money.

Money supply is increasing because of this, and that is OK really, nothing wrong with that. Loans usually result in increased value due to innovation product etc. The idea is not fundamentally flawed.

The problem with the current system is that while money for the loan principal is created out of thin air, the money for the needed interest payments to pay the loan back is not. And since the interest in not also created as part of the money creation: making money = making endless debt.

That really IS THE BIG BIG overlooked factor that sends global economy into crisis and debt spiraling.

Because it creates a musical chair situation. There is not enough money to pay all the debt there is. More loans have to be taken out to pay back loans, not good!

If you took all the money that existed in the world today it would not be enough (by a huge margin) to pay back all the money owed in the world. Pretty dumb actually.

The funny thing this whole system was created in the 17th/18th century and its based on an error (and no, I am not the first one who noticed).

But what I was proposing in 2019 was new:

**Just create the money for the interest payments along the money for the principal.**

Problem solved. Nothing else needs to change in the system, sanity rules, no more spiraling debt - finished.

Anyway, I presented this to lawyers and bank directors at the time and got some really nice feedback and some traction but I eventually gave up trying to get it implemented. It's just a too darn uphill struggle.

Because it has to be implemented on a big a scale to work. And for little me to convince the world on my own is difficult.

Funny enough the Feds, IMF and ECB are very well aware of this problem and know about it and are looking for solutions to stop the collapse.

In a strange way the Covid crisis helped because they were justified to give endless loans that the insolvency was stopped again - for a little while (but now inflation becomes a problem).

I want to take this whole idea into crypto now. Make a parallel currency that enables anyone to be a bank. Money is created by the repayments of loans (instead of at creation - because otherwise it will be abused and becomes a pyramid scheme).

The other thing that is fundamentally different to ordinary crypto: Normally you hold a ledger on the block chain. When you send money to someone it adds and subtracts.

I want to change that. I want to put actual coins on the chain (well actual tokens), that have nomination, can be printed (like a QR code) and taken with you and scanned by the receiver and thereby “transfered”.

The only thing that is on this part of the chain are tokens and their owners.

When you send money to someone there is no balance being carried. Just the owner of a token changes. Token ownership is secured by RSA key which you hold the private part of, just like in other coins. But some details still need to be sorted out.

What else is important is that tokens will have a lat/lon attached to them (or the id of a subchain they are part of). The idea being tokens can only be spent within a certain locality / vicinity (unless the owner moves the tokens to a new area).

So if I want to spend a token online in Japan, I have to first assign that location to the token **then** spend it.

The Reasoning for this is you only have a small section of nodes to check validity of a token owner and not the whole world, this allows for lightening block time and real POS (Point of Sale) / Retail transactions.

If you wanted to have all the tokens in the world on the chain it would become huge (like with bitcoin et all).

Idea is to have many local chains which interconnect. Might even use actual country or state borders for this. So a South African token has to be imported into the Swiss chain before it can be spend there.

Some people / organisation can opt to run full nodes, that have all the chains of the world downloaded and available and these nodes interconnect the local nets.

But if you just run a local wallet on your android /ios device you only have the local chain where you are about to spend your money.

If a coin is not transferred to a chain then then it can’t be spend there. This might also helps with security.

The localizing part is important because we don’t keep a ledger, we only keep the coins on the chain and the owners.

I am studying up on Ecliptic Curve Cryptography but I think, we need to stay away from Ecliptic Curves and rely on good old RSA with sufficiently long keys, or maybe, just maybe I could be convinced to use some curve that is unlikely to have an NSA backdoor in it.

What I am envision is we try to use technology that already exists. So full nodes would find each other and sync to each other using torrent like protocol but probably something over port 443 because that is mostly open.

I would propose to start with we keep the loan / repayment out of it and just concentrate on the coins itself and see how we can reach a consensus on ownership.

We seek consensus on which coin belongs to who. Every coin has his own keypair, so a mobile wallet holds pub/sec pairs for all the coins in the wallet.

We need to keep the block time low low low. Something like under 5 seconds would be good because it is perfect for POS (Point of Sale) / retail. Some other currency manage that. So it must be doable.

Because when you transfer a coin (which the user could print out theoretically as a QR code) you can verify if it's valid right away.

The transfer is just a way to give the secret key of the coin to the new owner. In case of a QR printout this this secret key would be protected by a PIN. So if you are in a shop, the salesperson scans your coins and then you need to enter your pin and the transaction is done.

The shop then has the public and private key of the coin and with that can rotate the keys and the coin is theirs, that is sort of how I envision it.

Each coin has to be verified on the block as being a valid coin. So each coin on the block would be a message containing the coin ID, the subchain (lat/lon) id, the secret key of the previous owner and a signature. Also the public key used to sign the whole message would be attached.

The fact that you have the private key makes you the owner. The new owner then has to create a new coin message and send it to the nodes to replace the old one. This new message is signed with his newly created pub/sec.

However since the message also contains the old private key other nodes can easily verify that replacement is indeed derived from the previous owner (by creating a signature on the previous entry with the private key given, if it matches the old sig then the private key was truly the one creating the sig and the transfer of ownership is valid).

This part is doable I am sure.

Then you broadcast the ownership change to all nodes you are in touch with. We have to see how other fast block currencies forms consensus but I think that is also doable.

Then there is another part here. Coins can be exchanged for coins of other denominations. If you have 100 coins in a domination of 1 and you want a single 100 coin you can destroy the 100 one coins for 1 time a 100 coin. This can also be proven, I am not seeing a big problem there either.

The tricky part is how money is created, we have to move real carefull here as it can spiral into a pyramid scheme if not carefull.

Here is what I envision:

Anyone can be a bank but you have to run a full node.

If you have a 100 coins and your neighbour wants to borrow 100 from you, you agree on interest (You negotiate that yourself, so the market makes the price of lending), and change ownership of your own 100 to the debtor (as part of a on-chain contract) (not like the banks now do with no security). That would give a pyramid scheme.

Each time a repayment is done ownership of coins is transferred back to the lender.

At the same time the same amount of money repaid is newly minted and distributed to the contributors of the currency (those that run full nodes).

It’s essentially a contract and it would be great if smart contracts would work for this currency too like e.g. an etherum.

Steps to achieve:

The first step would be to build the first part first without the loaning / creation. Simple coin based nodes. Even sub nodes/location should be left out, just simple, to show ownership transfer can be done on chain.

Since there is no ledger and each coin has its own key there is no ledger, privacy is assured and it's completely fungible.

If anyone reading this is interested, I would really appreciate getting in touch. I am trying to get a team together for this.

This is a currency which I believe could run parallel to current currency be really useful and save our bacon in a few years.

There will come a time when the current system will collapse. **Not if but when.**

And we don't want to end up with an "official" digital currency which is centralized, not private and is used to control population and enforce obedience.
