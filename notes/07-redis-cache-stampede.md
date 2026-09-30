# Redis Cache Stampede

Under high concurrency, many requests missing the cache at once can all hit the DB simultaneously. A short-lived lock (`SET key val NX PX 5000`) around the recompute step prevents the stampede.
