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

The idea behind this setup is to run the services you want on the machine that will be using them.  

For example if you are on a hotel network or public wifi.  

You can use this to regain a small amount of privacy without needing a full fledged VPN.  

[SearX search.](http://127.0.0.1)  
[PiHole Admin.](http://127.0.0.1:8080)   

Set your primary and secondary DNS servers to the following.

```
127.0.0.1
127.0.0.2
```

This is assuming you are running the docker containers on the machine that you are going to use the services on. Which is my intention.
