# DB Connection Pooling

Serverless functions can exhaust a database's max connections quickly since each cold start may open a new pool. A pooler like PgBouncer in transaction mode helps decouple app-level pools from real DB connections.
