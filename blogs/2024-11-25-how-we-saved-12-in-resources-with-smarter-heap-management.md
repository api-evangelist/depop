---
title: "How We Saved 12% in Resources with Smarter Heap Management"
url: "https://engineering.depop.com/how-we-saved-12-in-resources-with-smarter-heap-management-233f661e870d?source=rss----9d4f76b80a35---4"
date: "2024-11-25"
author: "Orji samuel"
feed_url: "https://engineering.depop.com/feed"
---
When we launched a new Scala service, we noticed memory issues as it gained usage. Key problems included: Memory usage increasing faster than expected, with some intermittent Out of Memory (OOM) errors Frequent garbage collection (GC) runs Uncontrolled memory usage until OOM To investigate, we took a heap dump using a free trial of this amazing tool called Jxray to analyze memory usage. Jxray revealed that we had underutilized buffers managed by the Netty framework, which was causing excessive memory usage.
