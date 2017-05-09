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

