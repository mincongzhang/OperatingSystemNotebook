## Benefits of Multithreading: CPU

![](/assets/threadings_in_cpu.png)

(1)t_idle:disk request, get data, disk respond
(2)CPU idle and wait
(3)if idle > 2*context switch, better let another thread do useful things
(4)if multi-processing, needs to create extra address space mapping(physical->virtual), very costly

1.Threads switch &lt; Processes switch

