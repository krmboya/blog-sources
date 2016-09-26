Title: Consistency Undervalued
Tags: distributed systems
      databases
      acid
      cap
PubDate: 2016-09-26
Description: On consistency being consistently undervalued

A short and sweet article [here](http://kevinmahoney.co.uk/articles/consistency-consistently-undervalued/) that discusses how guarantees in consistency of transactions
 can lead do simpler correct systems, and how, with the trend towards NoSQL databases and
 microservices, the industry has been abandoning the benefits provided by this guarantee.

Subsequent discussion on [hacker news](https://news.ycombinator.com/item?id=12519537)
with great points for both strict consistency and eventual consistency.

A point that emerges here is that for large distributed systems, there is a tradeoff
between high availability and strict consistency, and often system designers 
opt for high availability with eventual consistency.

The author of the article seems to advocate for maintaining strict consistency 
as much as possible, as this would lead to less buggy applications, and going for
eventual consistency where one can benefit from this, and clearly understands the
problem.

Some wikipedia links on applicable concepts in this discussion:

- [ACID (Atomicity, Consistency, Isolation, Durability)](https://en.wikipedia.org/wiki/ACID)
- [CAP (Consistency, Availability, Partition tolerance) theorem](https://en.wikipedia.org/wiki/CAP_theorem)
