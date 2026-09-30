# Graceful Shutdown in Node Services

On SIGTERM, stop accepting new connections first (`server.close()`), let in-flight requests finish, then close DB/queue connections — otherwise container orchestrators may kill the process mid-request during a rolling deploy.
