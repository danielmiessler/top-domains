# top-domains
A repository for maintaining a list of the top domains based on multiple lists

When Alexa (the domain list service, not the smart assistant) went away, it left a void.

Now there are a bunch of lists from places like:

- Cloudflare
- Ahrefs
- Semrush
- OpenDNS (Cisco)
- etc…

…that are providing their own.

But everytime I go to pull a list now, for a project like [Robots Disallowed](https://github.com/danielmiessler/RobotsDisallowed), I end up hunting around, not finding a good one quickly, and generally getting frustrated.

So this repo is going to be a place where I:

1. Store all those other lists in case you want them, and
2. Provide my own unified list that benefits from all of them

So basically if you just download [topdomains.txt](https://danielmiessler.com/), you should be good to go for most things you need. No fuss or muss.

## Methodology

So if you want to know about sausage, here's what I'm doing. Basically, newer lists are better, because the domains change all the time. But for projects like Robots Disallowed the order isn't super critical; what matters most is that the list is complete. But for other purposes, knowing which domains are **most popular** is the key information. So there you definitely want freshness.

The [topdomains.txt](https://danielmiessler.com) file gives you both.

What I do is take the best complete list I have at a given time, and then I take the best Top <code>N</code> entries from another list and bring those into the top of that larger list.

In other words, it's easier to get high-quality and very recent lists of like the top 10 domains, or even the top 100. But getting that for the top 1,000, or 100,000, or the full million, is much harder. 

This approach tries to get you the benefit of both the complete lists but also the absolute hottest top <code>N</code>.

