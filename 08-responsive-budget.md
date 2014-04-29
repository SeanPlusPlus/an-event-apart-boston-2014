# Responsive Design Performance Budget

Day two, eighth talk

https://twitter.com/paul_irish

The immediacy of touch interaction on phone makes ppl expect that page should load faster.

The #1 thing you can do to make site better on mobile is to make it faster

### Bloat

- has many meanings
- transfer size
- code complexity
- dead code

This looks good:

http://calendar.perfplanet.com/2013/an-engineers-guide-to-optimization/

### Bandwidth v Latency

- basically fewer resources better than smaller resources

### TCP Handshake

- whats up ... server says whats up back
- handshake incurs latency
- pingtime is the latency (for ex maybe 56 m/s if it is fast and 200 if it is mobile and slow)
- tcp slow start (4 packets then 8 then 16 ...)
- file concatentaion mitigates this
- tcp is optimized for open connections sending down a bunch of data
- *latency* is performance bottleneck for web, not bandwidth
- and mobile growth means more latency

### Critical CSS

- serve up less important stuff lower
- and crucial stuff in head and inlined
- optimize for the first crucial view

### Best practices

- move js to bottom
- minimize render blocking CSS
- deliver the goods (content should be in HTML - progressive enhancement)
- no redirects
- gzipping always helps
- visualize performance gains!
