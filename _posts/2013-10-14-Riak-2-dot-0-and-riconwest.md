--- 
title: Riak 2.0 at RICON West and the Emergence of a Market Leader
layout: newpost
summary: <p>The features and fixes coming to Riak in the 2.0 release will put it into another category of databases all together. RICON West will highlight a lot of this work and should be there to celebrate and discuss it with us.</p>
--- 

**October 15, 2013**

Before you read any further, go [buy a ticket](http://ricon-west-2013.eventbrite.com) for RICON West. There are only 10 left. 

[RICON West](http://ricon.io/west.html) is nicely-timed with the upcoming Riak 2.0 release. Though the code won't be official come October 29th, we'll have something testable - probably a "tech preview" - and people will get a feel for the features and functionality they can expect in production. We've got 23 [talks](http://ricon.io/west.html) in total happening at RICON West, covering the entirety of distributed systems. The Basho Team will be giving six, focusing primarily on what's planned in the new release [1]. Here's what you can expect from our developers:

### Data Types and the (forthcoming) End of Redis

The highlight of RICON West 2012 (for me) was when Sean Cribbs and Russell Brown stood on stage and [made a few numbers go up, down, and converge](https://vimeo.com/52414903) in front of 250 people. They were demoing Riak's then-nascent counters, a data type built on some magic called CRDTs. Since then, we've gone to great lengths to extend Riak's data type support, and 2.0 will feature a handful of structures intended to make the lives of developers everywhere easier; maps, sets, and registers are slated to be in 2.0 alongside counters.

[Sam Elliott](http://twitter.com/lenary), a whirlwind of an intern who hails from Scotch country, is [giving a talk](http://lanyrd.com/2013/riconwest/scmzrm/) that covers the current status of data types and why you should build applications on them. He worked alongside Sean, Russell, and a few others on the last leg of making data types official. We're not ready to displace Redis just yet, but if you've grown tired of writing custom logic to query a mess of Redis shards that are holding all your keys and values in RAM, this talk is for you. 

### Security

Riak has no security, something that doesn't sit well with some operators. This is understandable, and we recognized the need to build in something Basho-approved. For us it was always "when" not "if." About three months ago Andrew Thompson opened up an [issue against the Riak GitHub repo](https://github.com/basho/riak/issues/355) detailing our plans for adding security to Riak. It's a lively discussion and if you make it to the bottom you'll see links to a series of commits that will be in 2.0 as our first pass at security.  2.0 won't solve the entire security problem (it's a long road), and the first iteration only addresses security from the point of the client API, but this will be a strong first step for Riak.

Andrew's talk description is forthcoming but it's called [Riak Security; Locking the Distributed Chicken Coop](http://lanyrd.com/2013/riconwest/scpgbf/) and it will be a treat. Put it on your calendar. 

### Consistency is Hard but "Joe has a branch for that

A running joke at Basho is that Joseph Blomstedt, who goes by [jtuple](http://twitter.com/jtuple), "has a branch for that." But the best jokes are grounded in truth.  Joe [spoke last year](https://vimeo.com/51973001) about our ambitions for offering consistency on top of Riak, and [this year's installment](http://lanyrd.com/2013/riconwest/scmzrk/) will present the evolution of that work along with details on how and when you'll be able to use this code to build production services. 

### Revamped Full-text Search

Riak has long had indexing and search capabilities. 1.0 saw it become fully-integrated, and since then scores of companies have used Riak Search to build applications. [Bestbuy.com](http://http://bestbuy.com/), for instance, runs their inventory search system on it. Just over a year ago Ryan Zezeski [kicked off](https://github.com/basho/yokozuna/commit/bce28004900463aa665a866c35342a2569baedc8) something called Yokozuna. This is an effort to bring Riak and Solr closer together, enabling Basho and our community to make use of the many advancements that community has brought to the art and science of full-text search.  

Portland-based Basho Hacker [Eric Redmond](https://twitter.com/coderoshi) has been working alongside Ryan, Bryan Fink, and a few others to make Yokozuna production ready. If you're juggling Solr shards, rivers, or maintaining something homegrown you'll want to watch [Eric's talk](http://ricon.io/west.html#epicredmond). We're giving you the ability to run one cluster that handles both storage and full-text indexing and querying of documents. There are a few other pieces of open source technology that do this but Eric will show you why we're going to do it better.

### Supporting Riak in Production

Riak isn't perfect, nor are the environments in which people run it. To that end, Basho employs a team of savvy developers known as Client Services Engineers (CSE) who spend their time supporting our customers and community (in addition to writing code and tooling for Riak itself). If you've ever had the pleasure of dealing with them you know they possess a deep understanding of what it takes to run and fix Riak and other distributed systems in production. 

Justin Shoffstall and Charlie Voiselle, two members of the CSE team, are giving a talk called [The Seven-Layer Burrito; Troubleshooting a Distributed Database in Production](http://lanyrd.com/2013/riconwest/scpgbd/). Justin, Charlie, and the CSEs support F1000 companies running 100s of Riak nodes in production. They have invaluable experiences and data to share. Anyone running Riak in production (or planning to do so) should seek this talk out.

### Cluster Metadata - Riak's New Key/Value Store

Riak relies on a few different internal key/value stores to make some capabilities and features possible. (Yes. Very meta.) Riak 2.0 will have a revamped system for cluster metadata storage. Most users won't interact with it it directly, but it's a powerful addition to Riak's arsenal and will make things like the assignment and management of bucket properties much nicer. Jordan West's [Controlled Epidemics: Riak's New Gossip Protocol and Metadata Store](http://lanyrd.com/2013/riconwest/scpgrc/) talk will detail the work he and others have done on this subsystem. It's easily worth 45 minutes of your RICON time.

### Riak as a Market Leader

Blogs don't get read these days without some healthy hyperbole, so here it goes: the features and fixes coming to Riak in the 2.0 release will put it into another category of databases all together. There are no "Industry Firsts" to speak of, but we've expanded on our promise to be operationally-friendly while adding the richness and flexibility for which developers have been asking. (And there's a lot of other hotness in 2.0 not listed above.) If you've got a use case that involves operational, real-time workloads, I'm willing to bet this release can address it.  

[Join us](http://ricon-west-2013.eventbrite.com) at RICON West in a few weeks. This will be the largest gathering of the Riak community to date, and you'll be taking part in the evolution of our [once-humble key-value store](https://news.ycombinator.com/item?id=748079) that now powers thousands of applications at companies across the globe.

[Mark](http://twitter.com/pharkmillups)

[1] Per usual, all code is subject to ship early, late, or not at all.