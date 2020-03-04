# [http://dmitrysoshnikov.com/compilers/writing-a-pool-allocator/](Writing a Pool Allocator)
 * A Pool allocator (or simply, a Memory pool) is a variation of the fast Bump-allocator,
 * usually a pool allocator uses blocks of a predefined size.
 * Blocks and Chunks
    * A pool allocator operates with concepts of Blocks (Pools), and Chunks within each block.
    * Each chunk is of predefined size, and encodes the Object header, which stores a meta-information needed for Allocator’s or Collector’s purposes.

* Bump-allocate chunks 

### Let’s do a quick recap of the Pool allocator topic:
* It is used when we need to fast-allocate a lot of objects with predefined size
* Segregates heap by Blocks and Chunks
* Uses Bump-allocation for chunks within a block
* Allocates a new block on-demand when no chunks are left
* Fast deallocation: prepends a chunk at the front of the list
* Reuses freed chunks on future allocations
* Can deallocate a whole block at once if needed

## [CODE](https://gist.github.com/DmitrySoshnikov/07650cfb8f178cffe7276f96fd619008)
--------------------------------------------------------------------------------------

























