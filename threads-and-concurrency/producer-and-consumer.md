## Producer and Consumer Problem

![](/assets/producer_consumer_problem.png)

## Condition Variables

![](/assets/condition_variables_example.png)

NOTE for consumer:  
\(1\)Lock\(m\):The mutex is locked at the beginning  
\(2\)Wait\(m\):The mutex will be released, and re-acquired afterwards  
\(So that the producer can produce\)  
\(3\)Lock\(m\) ending:The mutex will be released again

![](/assets/condition_variables_api.png)

### Details of Wait()
Implemented in operating system threading lib:
(1)mutex released
(2)put to waiting queue of wait threads 
(3)notification received
(4)the thread will be removed from the queue
(5)mutex re-acquired and exit wait operation

NOTE for broadcast signals (notify_all):
notify_one: remove from queue and re-acquire mutex
notify_all: 
(1)remove all wait threads from queue
(2)wake up all threads at the same time
(3)but re-acquire the mutex one thread at a time and exit

So if you just want to wake up one condition, don't wake up all.