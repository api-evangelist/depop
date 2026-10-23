---
title: "Exploring Kafka Consumer At-Least-Once Delivery Guarantees: Expectations vs. Reality"
url: "https://engineering.depop.com/exploring-kafka-consumer-at-least-once-delivery-guarantees-expectations-vs-reality-36fd03e7a5e1?source=rss----9d4f76b80a35---4"
date: "2024-03-19"
author: "Jon Soul"
feed_url: "https://engineering.depop.com/feed"
---
Photo by Aaron Chavez on Unsplash Kafka is an event streaming platform that we use widely at Depop. From clickstream data to service-to-service communication; the ability to reliably produce and consume records to and from Kafka is fundamental to so many of the systems behind Depop. Yet recently, we uncovered some surprising consumer behaviour in one of our services that made us rethink how we understand one of the core concepts of event-driven systems and how it applies to our use of Kafka across our platform.
