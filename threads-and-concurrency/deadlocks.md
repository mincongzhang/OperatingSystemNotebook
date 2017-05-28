## Deadlocks

Definition: Two or more competing threads are waiting on each other to complete, but none of them ever do.

How to avoid:
(1)Use a big mutex
(2)Maintain lock order