---
title: "How Fast Is DoltLite?"
url: "https://dolthub.com/blog/2026-06-08-how-fast-is-doltlite/"
date: "2026-06-08"
author: "Tim Sehn"
feed_url: "https://www.dolthub.com/blog/rss.xml"
---
A couple months ago, we released DoltLite , a free open-source drop-in replacement for SQLite with Dolt -style version control features. DoltLite works by ripping out SQLite’s B-Tree storage engine and replacing it with a content-addressed Prolly Tree , the same data structure that powers Dolt. We’ve been benchmarking Dolt against MySQL for years using sysbench . Recently, Dolt got faster than...
