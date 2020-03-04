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


# EXPLORE
## [Essentials of Garbage Collectors](http://dmitrysoshnikov.com/courses/essentials-of-garbage-collectors/)
https://os.phil-opp.com/allocator-designs/

## Memory layout https://www.youtube.com/channel/UC15UOu9F157NAXGL9dHc4TQ/videos
Writing a Memory Allocator http://dmitrysoshnikov.com/compilers/writing-a-memory-allocator/#video-lecture

Page Tables https://os.phil-opp.com/page-tables/

https://os.phil-opp.com/paging-introduction/


Operating Systems: Three Easy Pieces
http://pages.cs.wisc.edu/~remzi/OSTEP/


Educational Memory Manager and set of Garbage Collectors


https://github.com/DmitrySoshnikov/mmgc
threads
https://github.com/DmitrySoshnikov/threads
https://solarianprogrammer.com/2011/12/16/cpp-11-thread-tutorial/



angrave
/
SystemProgramming
https://github.com/angrave/SystemProgramming/wiki

MIT 6.004 L15: The Memory Hierarchy
https://www.youtube.com/watch?v=M7DxxD0x4bg








