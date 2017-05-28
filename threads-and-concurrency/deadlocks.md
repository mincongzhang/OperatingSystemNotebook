## Deadlocks

Definition: Two or more competing threads are waiting on each other to complete, but none of them ever do.

### Example

Two threads are waiting each other in a circle





How to avoid:  
\(1\)Use one MEGA mutex  
\(2\)Maintain lock order

