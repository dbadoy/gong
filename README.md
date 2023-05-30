# gong
This helps translate papers by copy-pasting text.

https://www.dbadoy.dev/gong/


<-- Example text in papers
```
Before discussing the details of our anti-caching model, we first
review H-Store’s architecture and the motivations behind its design.
In a disk-oriented DBMS, the system retrieves tuples from blocks on
disk as they are requested by transactions. These blocks are stored
in an in-memory buffer pool. If a transaction invokes a query that
accesses data that is not in memory, the DBMS stalls that transaction
until the block with that data is retrieved from disk and added to the
buffer pool. If the buffer pool is full, then the DBMS chooses another
block to evict to make room for the incoming one. Since the transaction
waits until this disk operation completes, such systems employ a
concurrency control scheme to allow other transactions to execute while
the stalled one is waiting for the disk. The overhead of this movement
of data and coordination between ...
```

--> Result
```
Before discussing the details of our anti-caching model, we firstreview H-Store’s architecture and the motivations behind its design.In a disk-oriented DBMS, the system retrieves tuples from blocks ondisk as they are requested by transactions. These blocks are storedin an in-memory buffer pool. If a transaction invokes a query thataccesses data that is not in memory, the DBMS stalls that transactionuntil the block with that data is retrieved from disk and added to thebuffer pool. If the buffer pool is full, then the DBMS chooses anotherblock to evict to make room for the incoming one. Since the transactionwaits until this disk operation completes, such systems employ aconcurrency control scheme to allow other transactions to execute whilethe stalled one is waiting for the disk. The overhead of this movementof data and coordination between ...
```
