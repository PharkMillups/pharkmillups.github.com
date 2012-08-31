--- 
layout: newpost
title: Towards A Community Of Distributed Systems Developers 
summary: <p>RICON is our first opportunity to bring together a community of distributed systems developers in the flesh. And we're damn excited about it.</p> 
--- 

**August 31, 2012**

Pat Helland's 2007 position paper [Life beyond Distributed Transactions: an Apostate's Opinion](http://cs.brown.edu/courses/cs227/papers/weaker/cidr07p15.pdf) includes the following paragraph in the abstract (in reference to the purpose of the paper):

> 
The reason for starting this discussion is to raise awareness of new patterns for two reasons.  First, 
it is my belief that this awareness can ease the  challenges of people hand-crafting very large 
scalable applications.  Second, by observing the  patterns, hopefully the industry can work  towards the creation of platforms that make it easier to build these very large applications.
>

This closely parallels what Basho is attempting to build with developers writing and deploying scalable systems. If you have more than one machine, you have a distributed system, and this changes things. The Basho team lives and breathes distributed systems - both at the software and [company level](http://www.themarkphillips.com/2011/06/27/Building-and-Maintaining-Internal-Community-And-Culture.html) - and though Riak is our preferred method for storage, retrieval, and querying of data over N machines, we have a passion for sound distributed fundamentals at the lowest level possible. There are many good technologies in the realm of data storage. Riak is just one of them. 

For the past three years or so we've been using [Riak](http://wiki.basho.com/Riak.html) as the binary embodiment of our beliefs in how distributed data storage should function. In addition to actual software, we've used other methods like [blogs](http://basho.com/blog), meetups [ [1](www.meetup.com/BashoChats/) [2](www.meetup.com/San-Francisco-Riak-Meetup/) ], and [presentations](http://www.infoq.com/presentations/Things-Break-Riak-Bends) to get this message across. We now have the opportunity to do so with a proper conference: [RICON2012](http://ricon2012.com)

In that vein, I recently had an exchange with [Marco Gallotta](https://twitter.com/marcog) in which he asked if it would be valuable for him to attend even though he wasn't using Riak:

<blockquote class="twitter-tweet" data-in-reply-to="240517533164240896"><p><a href="https://twitter.com/marcog"><s>@</s><b>marcog</b></a> Absolutely. Riak will be a focus, but we're trying to cultivate an awareness of hard problems that come along with all dist. dbs</p>&mdash; Mark Phillips (@pharkmillups) <a href="https://twitter.com/pharkmillups/status/240517971448066048" data-datetime="2012-08-28T18:35:27+00:00">August 28, 2012</a></blockquote>
<script src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

My response (pardon the typo I just discovered) sums up what we're trying to do with RICON. There are no silver-bullet, physics-defying databases. There are only tradeoffs and the design decisions you need to make when taking them into account. Most (if not all) of the talks from the [presenting community members](#) (be they Riak users or otherwise) will not be 100% positive. No one at Basho is reviewing slides or censoring talks. [Speakers](http://basho.com/community/ricon2012/#speakers) will be giving honest accounts of the good and bad aspects of using distributed systems in production. This is why we've asked awesome speakers like [Selena Deckelmann](htt://chesnok.com/) to come talk about PostgreSQL; and Dana Contreras to talk about [how Twitter rebuilt itself](http://lanyrd.com/2012/ricon2012/oct-10/) on the fly; and Joseph Hellerstein to talk about new, powerful tools [like BLOOM and CALM](http://lanyrd.com/2012/ricon2012/sxggb/) that could (and will) open up new doors for developers.

[Come to RICON](http://ricon2012.eventbrite.com) if you love HBase and want to tell the world why it's the best column store available today; if you think Cassandra is the future of databases; if you have 1TB of data in Redis and are considering writing your own sharding logic. As my colleague jtuple [pointed out yesterday](http://gist.io/3541459), there will be plenty of content on the future of Riak, but on the whole we're doing our part to convene a community of developers and architects who want to apply what academia has been excited about for many years. Come to RICON to be a part of this. It's our first opportunity to bring the community together in the flesh, and we're damn excited about it. 

[Mark](http://twitter.com/pharkmillups)
