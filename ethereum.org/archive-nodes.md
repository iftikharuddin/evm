# Archive Nodes

Think of Ethereum's data like a photo album:

Regular Node (Full Node):
- Keeps latest photos (current state)
- Only few recent snapshots
- Can recreate old photos but takes time
- Uses less storage (~400GB)

Archive Node:
- Keeps EVERY photo ever taken
- All historical states saved
- Instant access to old data
- Uses lots of storage (3-12TB)

Main Uses:
1. Quick access to historical data like:
- "What was Alice's balance 6 months ago?"
- "What happened in this contract last year?"

2. Useful for:
- Block explorers
- Researchers
- Security analysts
- Developers
- Auditors

Hardware Needs:
- Lots of storage (3-12TB)
- Fast SSD drives
- Good CPU for initial setup
- Takes up to a month to sync

Important Points:
- Regular users don't need archive nodes
- Network doesn't depend on them
- They're just for convenient historical access
- Erigon client is most efficient (needs only 3TB vs 12TB)

Think of it like this: A regular node is like having today's newspaper, while an archive node is like having every newspaper ever published, neatly organized for quick reference!