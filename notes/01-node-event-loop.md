# Node.js Event Loop

The event loop has 6 phases: timers, pending callbacks, idle/prepare, poll, check, close callbacks. `setImmediate()` runs in the check phase, after I/O events in the poll phase, which is why it usually fires before a `setTimeout(fn, 0)` scheduled at the same tick.
