# cluster vs worker_threads

`cluster` forks separate OS processes with separate memory (good for scaling HTTP servers across cores); `worker_threads` share memory via `SharedArrayBuffer` and are better suited to CPU-bound work within one process.
