# learn-spark

## RDD : resilient distributed dataset
- distributed / partitioned
  - split across nodes in the cluster
- immutable
  - new RDD is created whenever actions are performed on it 
- resilient 
  - is available even if the underlying node is not.
- operations 
  - read : `take` provides a way take certain number of elements from the RDD while `collect` will capture the entire set.
  - transformation : multiple transformations can be performed. each produce a new RDD. A RDD remembers the `lineage` from which it comes from, all the transformations are in memory and do not apply until the results are accessed (persisted to screen or file)
  
