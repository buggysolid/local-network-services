# What

A docker compose file that brings up pihole, unbound and searx.

What do I get?

- An authorative adblocking DNS server.
- Heavy DNS caching with prefetching.
- Serving from stale cache. (You will get DNS answers in the case that upstream is having issues.)
- A search engine that caches results from Google, Bing, Yahoo ect.

# Requirements

[Docker](https://docs.docker.com/engine/install/) 

# Run

```
git clone https://github.com/buggysolid/local-network-services
cd local-network-services
docker-compose up -d
```

# Use

[SearX search.](http://127.0.0.1:8080)  
[PiHole Admin.](http://127.0.0.1)   
