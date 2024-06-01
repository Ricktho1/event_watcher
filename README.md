# Event watcher contract examples

## Quick Start

```bash
# Run event watcher http
cargo run --bin event-watcher-http

# Run specific block number event watcher
cargo run --bin specific-block-event-watcher

# Run event watcher websocket
cargo run --bin event-watcher-ws

# Run event watcher http and send to discord
cargo run --bin event-watcher-http-discord
```

#### The event log, the topics field has 3 values:

```bash
topics[0] is the keccak-256 of the `Transfer(address,address,uint256)` canonical signature.
topics[1] is the value of the `_from` address.
topics[2] is the value of the `_to` address.
```
