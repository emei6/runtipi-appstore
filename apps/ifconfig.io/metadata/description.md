# ifconfig.io

Inspired by ifconfig.me, but designed for pure speed. A single server can do 18,000 requests per seconds while only consuming 50megs of ram.

## Short Summary

I used the gin framework as it does several things to ensure that there are no memory allocations on each request, keeping the GC happy and preventing unnessary allocations.

Tested to handle 10,000 clients doing 90,000 requests persecond on modest hardware with an average response time of 42ms. Easily servicing over 5 million requests in a minute. (Updated June, 2022)
