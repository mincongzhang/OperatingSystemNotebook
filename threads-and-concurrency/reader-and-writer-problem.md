## Readers and Writer Problem

\(1\)multiple readers and one writer, access one file  
\(2\)Simple solution: add a mutex to control reading and writing to the file  
\(3\)Problem: one reader is reading, other readers cannot read  
\(4\)Solution: Use a proxy resource, and use mutex to control the resource

![](/assets/readers_and_writer_problem.png)



