---
title: Applications over the internet
date: 2020-05-22T05:44:33+01:00
draft: false
---

When I started using a computer, most software did not require a connection with the internet, I would spend most of my time playing around the computer itself. Internet was something expensive and almost impossible to use as a kid. These days we have the opposite, everything is online, even text editors and similar software. More and more we are losing that ability and relying on "Software as a Service". For non-techies the difference may not even be clear. The software runs on the cloud and that's it. But what's the cloud? (tip: it's a computer owned by someone else). 

There are different approaches on how to set up a network application. The most common one today is the centralised approach, where you use a client on your computer (computer, mobile phone, smartwatch, whatever)  and requests content to a server in the internet. For example, you have to visit Youtube to be able to see that cute cat video your friend told you about: you request the video and download from Youtube’s computers. Although this is the most common way we use the internet these days, it’s not the only one possible. One example is the Peer to Peer, where you can download movies from different computers spread over the internet. 

Every single architecture has its tradeoffs, especially regarding security and privacy. In a world where some get richer by making the information we generate a private property, we should do all of our decisions knowing the price and risks we pay.
# Centralised approach

This is the most common approach these days, you pay for a service and you can access its software hosted “on the cloud” (a corporation computer). Being Netflix, some fancy task tracker, or a budget system. The way you pay can be either in money format or by accepting them to use the information you gave to do whatever they find useful.  The company owns the software that holds your data.

Your computer acts like a client and sends requests to the server (i.e. gmail website). The server processes your inputs and gives you an output. For example, when you send your message to Twitter server (computer), it stores it to show later to your followers. In this case Twitter is holding YOUR data in THEIR servers. Another example is when you access (request) twitter home page, twitter will return the content the people you are following posted.

This is normally the easiest way to use something since it requires almost zero knowledge. You can access everywhere. The cons here are that unless you read the whole terms of the agreement, you are not sure what they are doing with the information you input (give) in their system. Do they feed an AI system? Do they allow employees to read your data? Do they share your data with a third-party? Do they share with governments?

In Europe, the [GDPR](https://ec.europa.eu/info/law/law-topic/data-protection/data-protection-eu_en) helps to alleviate a bit this, with a set of rules defined by the EU on how your data must be stored, used, and purged.


## Self-hosted

Instead of using someone else's computer to run those centralised software, you can host yourself. This normally requires a lot of attention, since mistakes may open your data to attackers. There are approaches trying to simplify this. Like the [FreedomBox](https://freedombox.org/), a small computer that according to their own website: "empowers its users to avoid the data mining, censorship, and surveillance by centralised silos that characterise the web of today. It makes web servers personal, affordable, and manageable so that a user can host necessary web services at home on a device they own, powered by free software they can trust.".

If correctly set up, you can also access this from everywhere, and you own your data. The problem is that you also own the maintenance of it: making sure you have backups or being ok to not access the service if there are issues with the local internet provider or with the electricity supply.

You can also self-host in the cloud, you must still take security measures to make sure no one can access your data. This is the case of this blog as I write this, though I have plans to start using my own computer to host it in the near future.

There are also some collectives hosting different software and giving access to individuals. Like [Systemli](https://www.systemli.org/en/index.html).

# Peer to Peer and decentralised

On Peer to Peer (P2P) systems you don't have a central server responsible for the application. Each client also works as a “server”. The most common example is torrent. You can stream movies using the data stored in other people computers instead of Netflix computers. The data is distributed between different computers and even if a government tries to censorship a country or a website, it’s very hard to kill that content, since everybody that saw it may be distributing as well. In other words, P2P applications allow you to share content without holding a server (in the sense of a centralised computer), the protocols must be secure or you must be fine with random people being able to read the contents. So you basically have some clues since the beginning if the protocol is safe or not.

Let’s keep thinking in the torrent example, in a very simplified way: (1) you request pieces of the file to everyone that have it in theirs computer; (2) meanwhile you are also sharing the pieces you have in your computer with other people. The data is owned by all those people involved in that conversation. 

P2P are not only to download torrents. There are more complex usages like [IPFS](https://ipfs.io/), "a peer-to-peer hypermedia protocol designed to make the web faster, safer, and more open". Today there are a lot of people studying and hacking new ways to use P2P applications, a lot of people believe this is the future we want for the internet, where the Big Tech companies don’t hold all the power.

The decentralised may also look very similar to a client-server environment. [Mastodon](https://mastodon.social/about) is a Twitter alternative that’s distributed although it does not really use P2P as the torrents use. The approach here is different, everyone is free to install their own instance (server) of Mastodon, and “using a suite of standard protocols, Mastodon servers can exchange information with each other, allowing users to interact seamlessly.”. In other words, if someday something happens with the instance you were using, you are free to spin up your own, or maybe create one with only your friends, so you are sure you will not be target by ads depending on what you write there.
# Where this leaves us?

Here is a table showing who is responsible for the data you insert into the network application for each architecture I showed:

* &#128022; = Corporations;
* &#128038; = People over the internet;
* &#128025; = User (you);

|       |Your Data |
| -----------| ----------- 
|Centralised &nbsp;&nbsp;&nbsp;| &#128022; |
| Self-hosted&nbsp;&nbsp;&nbsp;&nbsp;|&#128025;   |
| Self-hosted using the cloud&nbsp;&nbsp;&nbsp;|&#128025; + &#128022; |
| P2P        | &#128038; + &#128025; + &#128022;  &nbsp;&nbsp;&nbsp;&nbsp; |



# Learn more about the subject

1. [Telekommunist Manifesto](https://wiki.p2pfoundation.net/Telekommunist_Manifesto)
2. [Peer to peer: a commons manifest](https://commonstransition.org/peer-to-peer-a-commons-manifesto/)
3. [Decentralisation: the next big step for the World Wide Web](https://www.theguardian.com/technology/2018/sep/08/decentralisation-next-big-step-for-the-world-wide-web-dweb-data-internet-censorship-brewster-kahle)