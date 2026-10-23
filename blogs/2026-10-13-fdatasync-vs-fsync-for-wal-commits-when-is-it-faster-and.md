---
title: "fdatasync vs. fsync for WAL commits: When is it faster and what are the tradeoffs?"
url: "https://dolthub.com/blog/2026-10-13-overwrites-and-fdatasync-vs-fsync/"
date: "2026-10-13"
author: "Aaron Son"
feed_url: "https://www.dolthub.com/blog/rss.xml"
---
Dolt's WAL commit implementation on Linux recently changed from fsync to fdatasync. Internal sysbench runs showed a big improvement. What are the tradeoffs?
