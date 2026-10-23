---
title: "How we cut our largest Spark pipeline’s cost by 52%"
url: "https://engineering.depop.com/how-we-cut-our-largest-spark-pipelines-cost-by-52-014faa81d179?source=rss----9d4f76b80a35---4"
date: "2026-08-11"
author: "tommywatts"
feed_url: "https://engineering.depop.com/feed"
---
Co-authored by tommywatts and Tommaso Peresson Freshness had doubled twice in a few years, from twice a day, to four times, and now eight. The pipeline code itself never changed, but every run repeated work the previous one had already done, and this started to get expensive. We call this Silver Ingest, our largest data ingestion pipeline, sitting at the core of a medallion -structured data lake, a common tiered data organisation strategy that transforms raw “bronze” events into refined “silver” tables, which contain data that is exactly deduplicated, compacted, and optimised for high-performa
