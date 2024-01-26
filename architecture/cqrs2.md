---
layout: module-with-evals
badge: B2t1_gr2R_6e4kHYkEy0oA
level: 0
title: CQRS Developer 2
parent: Architecture
nav_order: 5
description: A developer who can build systems that take advantage of the segregation of commands and queries, including event sourcing.
---

## Master the following skills:

- Write aggregate methods that generate domain events
- Write an event sourced and invariant aggregate using a stream of domain events
- Broadcast domain events upon persisting the domain aggregate
- Handle domain events with event handlers
- Persist domain events to a database
- Write idempotent projections to update a view store when changes occur
- Explain the impact of CQRS on Consistency, Availability and Scalability
  of the system
- Implement Snapshotting of an aggregate to reduce the time it takes
  to handle a Command
- Write unit tests for domain event handlers
- Run a complete workflow from endpoint request (PUT or POST) to "eventually consistent" view store to the UI
- Discuss what types of tasks should be handled in a command handler vs aggregate vs domain event handler vs domain service

## Suggested Learning:

- [Introduction to CQRS and Event Sourcing](https://eventsourcery.com/){:target="\_blank"}
- [Video course: Event Sourcing, Distributed Systems & CQRS](https://www.youtube.com/playlist?list=PLEV9ul4qfGOZ5gWIPMlFGMUpenSs1EvxZ){:target="\_blank"}
- [Event Sourcing Projections Patterns: Deduplication Strategies](https://domaincentric.net/blog/event-sourcing-projection-patterns-deduplication-strategies){:target="\_blank"}
