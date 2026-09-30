# Node.js Streams Backpressure

If `stream.write()` returns `false`, you must wait for the `'drain'` event before writing more — ignoring backpressure can balloon memory usage when the writable side is slower than the readable side.
