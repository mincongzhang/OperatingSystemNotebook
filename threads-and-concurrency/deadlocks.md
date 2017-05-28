## Deadlocks

Definition: Two or more competing threads are waiting on each other to complete, but none of them ever do.

### Example

Two threads are waiting each other in a circle![](/assets/deadlocks1.png)

![](/assets/deadlock2.png)

How to avoid:  
\(1\)Use one MEGA mutex  
\(2\)Maintain lock order \(first A then B\)  

### Summary

A cycle in the wait graph is __necessary and sufficient__ for a deadlock to occur (edges from thread waiting on a recources to thread owning a resource)

#### What to do about deadlock?

(1)Deadlock prevention - Expensive  
(2)Deadlock detection & recovery - Rollback  
(rollback execution, maybe impossible to perform)  
(3)Do nothing...