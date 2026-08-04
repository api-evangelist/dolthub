---
title: "Running Ito, a Runtime Analysis Code Review Tool, on Doltgres"
url: "https://dolthub.com/blog/2026-07-20-ito-ai-qa-for-doltgresql/"
date: "2026-07-20"
author: "Jason Fulghum"
feed_url: "https://www.dolthub.com/blog/rss.xml"
---
For the past six weeks, we've been running Ito, a runtime analysis code review tool that works off of GitHub PRs and builds and runs your application instead of just reading the diff. We've had success using this on our Doltgresql repo and in this blog post we'll show what it's caught, how it works, and where it's let us down.
