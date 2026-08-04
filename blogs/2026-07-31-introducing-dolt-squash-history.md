---
title: "Introducing `dolt_squash_history()`"
url: "https://dolthub.com/blog/2026-07-31-squash-history/"
date: "2026-07-31"
author: "Tim Sehn"
feed_url: "https://www.dolthub.com/blog/rss.xml"
---
Dolt keeps every version of every row, but sometimes you want less history, not more. The new dolt_squash_history() procedure collapses your commit history into a single commit with one call, no rebase required. This article explains why and how.
