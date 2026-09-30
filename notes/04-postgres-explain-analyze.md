# Postgres EXPLAIN ANALYZE

`EXPLAIN (ANALYZE, BUFFERS)` shows real execution time and buffer hits/misses, not just the planner's estimate. Always run it against production-sized data — the planner picks different strategies at different table sizes.
