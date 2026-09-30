# HTTP Idempotency Keys

For POST endpoints that create resources (like payments), accepting an `Idempotency-Key` header and caching the response by that key prevents duplicate side effects on client retries.
