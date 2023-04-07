Hacker News (unofficial) API
============================

Yet another unofficial API for [Hacker News](http://news.ycombinator.com/).

- API (Cloudflare CDN, faster response time): <http://api.xdv.com/>
- API Documentation: <https://github.com/davelevine/node-hnapi/wiki/API-Documentation>

---

🚧 PLEASE READ THIS 🚧
---

If you are planning to scrape a *huge* amount of posts or (historical) data from HN, please **don't use this API**. Use the official [Hacker News API](https://github.com/HackerNews/API) or [HN Search API](http://hn.algolia.com/api) instead.

---

Quick Start
----------

1. `git clone` this repo.
2. `cd` to repo folder.
3. Optionally download, install and start [redis](http://redis.io/download).
4. `npm i`
5. `npm start`
6. Load `localhost:1337` in your web browser.


Example
-------------

> <http://api.xdv.com/news?page=2>

Configuration
-------------

HNapi uses [dotenv](https://github.com/motdotla/dotenv) for configuration.

- `PORT` - (default: `1337`) Server port
- `CACHE_EXP` - (default: `600`) Cache expiry in seconds
- `LOG_REFERER` - (default: `false`) Logs referers
- `LOG_USERAGENT` - (default: `false`) Logs user-agent strings
- `CACHE_MEMORY` - (default: `true`) Use in-memory caching
- `CACHE_STORE` - (`redis`, default: none) Specify the cache store
- `CACHE_SERVER` - `HOST:PORT` for Redis server

License
-------

Licensed under the [MIT License](/node-hnapi/LICENSE).

Other APIs
----------

- [The official Hacker News API](https://github.com/HackerNews/API)
- <http://hn.algolia.com/api>
- <http://api.ihackernews.com/>
- <http://hndroidapi.appspot.com/>
- <http://www.hnsearch.com/api>
- <https://github.com/Boxyco/hackernews-api>
