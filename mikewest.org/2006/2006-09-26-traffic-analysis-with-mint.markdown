---
Alias:
- http://mikewest.org/blog/id/34
Modified: '2006-09-26T17:13:36Z'
Teaser: I use Mint to analyze the traffic on this website.  It's a powerful tool,
    made more powerful with some excellent plugins.
layout: post
tags:
- Personal
title: Traffic Analysis with Mint
---
Like most people with personal websites, I'm hugely interested in my stats.  This is fairly laughable, given the hugely unimpressive number of hits I get a day, but I'm interested regardless.

Generally speaking, I care about two things: who's pointing to my posts (referrers), and how many people are hitting the site (visits).  [Egosurfing Technorati][ego] is a nice way of getting some of this information, but it just doesn't feel very accurate, and it simply can't be as detailed as some other solutions that actually integrate themselves into your site.  Let's talk about one of those that I've found useful: [Shaun Inman][shaun]'s [Mint][mint].

[shaun]: http://www.shauninman.com/
[mint]: http://haveamint.com/ "Mint: A Fresh Look at Your Site"
[ego]: http://technorati.com/search/mikewest.org "Technorati Search: 'mikewest.org'"

When it comes to elegant display of the ebb and flow of your site's current traffic, I haven't come across anything better than [Mint][].  In it's default configuration, I don't think it's a robust solution for high-traffic sites (loading the dashboard alone practically tanks [Digital Web][]'s server), but it's pure magic for a personal site like this one.

[digital web]: http://www.digital-web.com/ "Digital Web Magazine"


Out of the box, [Mint][] gathers and presents several bits of information that I care about.  Adding a few key plugins, or "Peppers" (Pepper.  Mint.  Peppermint.  Oh that clever guy...), expands the default functionality to encompass almost everything else I care about.  In fact, [the community][forum] that's sprung up around Mint is really the reason Mint is worth the $30 to me.  The high level of interest and interaction practically ensures that a Pepper will spring up when a new idea floats around for improving analysis ([Peppermint Tea][peppers] gathers these plugins together in a decent way, so they're always fairly easy to find).

[forum]: http://haveamint.com/forum/ "Mint Support Forum"
[peppers]: http://www.massiveblue.net/pepperminttea/

## Aggregate Numbers ##

Mint gives me a lot of insight into the current patterns of traffic on my site.  Specifically, it provides a __day-by-day view of my aggregate hit numbers__.  I like seeing numbers, and the default installation of Mint does a nice job presenting the total number of page views, and a reasonable job guessing at the total number of _unique_ visitors.  It runs via a JavaScript include, and sets a cookie on each visitor's browser, so I'm much more confident in this tatter number than I am in the numbers generated by a log analyzer like [AWStats][].

[awstats]: http://awstats.sourceforge.net/ "AWStats - Free Log File Analyzer"
    
The default Peppers are good at displaying the raw numbers, but to really get a grasp on the traffic information, [Kyle Rove][] has put together a brilliant Pepper called [Fresh View][] that renders the totals and uniques as an SVG-based graph.  It's _pretty_, and absolutely increases my ability to _analyze_ the information in a useful way.  Looking at a little dot that's twice as high as the previous dot means something to me _immediately_ about my traffic patterns; raw numbers simply don't have that impact.

[kyle rove]: http://www.sensoryoutput.com/ 
[fresh view]: http://www.sensoryoutput.com/projects/freshview/ "Fresh View for Mint"

More than daily numbers, I find it really interesting to see the trends that pop up when comparing day to day traffic.  [Brett DeWoody][brett] and [Ronald Heft][ronald] put together the cleverly named [Trends][] Pepper that's surprisingly good at processing the raw traffic data, and presenting useful trending information that you can actually do something with.  I have mine configured to compare the previous 7 days of traffic to the 7 days before that, which gives me a pretty accurate picture of which posts people are reading _now_, compared to which posts they were reading a week ago.  I get the same information about referrers and searches, all with one Pepper.  It's really quite well put together, letting you dive into the information to see the history on a day-to-day basis for closer examination.  I'm really happy with how it performs.

[brett]: http://brettdewoody.com/
[ronald]: http://cavemonkey50.com/
[trends]: http://cavemonkey50.com/code/trends/ "Trends"
    
## Referrers ##

Pure traffic numbers are great, and I enjoy seeing my traffic move around and the way that trends pop up now and then, but my _real_ curiosity is all ego: who's talking about me, and what are they saying?  [Links are the lifeblood of the web][praise], and I'm _very_ interested in who's sending traffic my way.  Mint, of course, tells me.

Out of the box, Mint captures referrer information, and gives me a list of the newest unique incoming links.  Even better, it gives me an RSS feed of the newest unique referrers, so I don't have to reload the Mint dashboard every five minutes to feed my data addiction; I just pop open [NetNewsWire][] and there they are.  Brilliant stuff.  

Of course, new unique referrers aren't all I care about.  I'm also curious about the long-term links from more popular pages that just keep driving traffic in.  Mint does collect counts for repeat referrers, but the [Trends][] Pepper mentioned above fills in the details much more nicely, giving a good overview of who's sending traffic _now_ vs. _before_.

## Search Results ##

The last thing I want to see are the keywords and phrases that are driving people to my site.  I want to know _how_ they find me, and what they were looking for, mostly because it gives me ideas for new articles and provides important information about the _words_ that are important when describing certain topics.  If I continually write about unobtrusive JavaScript techniques, but never say the word "AJAX", then I'm missing out on an easy way to optimize my content for search engines.  And when I see that the articles I wrote about [prepping for technical interview questions][prep] are getting some good traffic, it's an inspiration to write more on the topic.  I _like_ the idea of people _actually reading_ what I write; knowing what people are looking for when they find me is a good step in that direction.

And hey, every once in a while, people search for things like "mike west is number 1", which I like to pretend is _really_ about me.

## Alternatives ##

Mint isn't the only analysis package out there, and $30 is a bit steep for it's functionality on just one site, really.  So what else might you look at to get some of the power of Mint at a lower price?  These are some that I've used:

*   [Google Analytics][ga] is a nice system that Google's put out for free. 
    It's a little obtuse to use, and is really more focused on the needs of
    high-end users that want to optimize their ad spend than on the needs of
    personal websites.  That said, it's free, and it really does work pretty
    well.  It's just not as elegant as Mint.
    
*   [SlimStat][] is an analytics engine based on a precursor to Mint:
    ShortStat.  Shaun Inman released ShortStat under the GPL before moving on
    to write Mint, and [Stephen Wettone][] took off and ran with it, building
    in a lot of nice functionality, and building up a [good-sized
    community][slimstatgroup] at the same time.  It's not as polished as Mint,
    and lacks the real plugin architecture that makes Mint so appealing to 
    developers, but it's a solid, free alternative that's well worth taking a
    look at.

[ga]: http://analytics.google.com/
[slimstat]: http://wettone.com/code/slimstat "SlimStat"
[slimstatgroup]: http://groups.google.com/group/slimstat "SlimStat Google Group"

[prep]: http://mikewest.org/archive/answers-to-common-interview-questions "Mike West: Answers to Common Technical Interview Questions'"

[praise]: http://adactio.com/articles/1132/ "Jeremy Keith: 'In Praise of the Hyperlink'"
[netnewswire]: http://ranchero.com/netnewswire/ "NetNewsWire"
[stephen wettone]: http://wettone.com/ "Stephen Wettone"


