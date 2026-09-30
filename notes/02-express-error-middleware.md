# Express Error Middleware

Error-handling middleware in Express must be defined with 4 arguments `(err, req, res, next)` even if `next` is unused — Express detects error middleware by arity, not by name.
