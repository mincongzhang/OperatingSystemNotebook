## Readers and Writer Problem

\(1\)multiple readers and one writer, access one file  
\(2\)Simple solution: add a mutex to control reading and writing to the file  
\(3\)Problem: one reader is reading, other readers cannot read  
\(4\)Solution: Use a proxy resource, and use mutex to control the resource

![](/assets/readers_and_writer_problem.png)

### Example

![](/assets/readers_and_writer_example.png)

```
//In writer:

while(resouce_counter!=0){
    Wait(counter_mutex,writer_phase);
}

//(1)the waiting process is not atomic. 
//(2)While it's waiting, the mutex will be released.
//(3)And when it gets writer_phase signal, meanwhile, there may be another reader locks the mutex and increment the counter.
//(4)So we have to check the counter again.

Broadcast(read_phase);
Signal(write_phase);
```

### Critical Section Structure

![](/assets/reader_writer_structure.png)

