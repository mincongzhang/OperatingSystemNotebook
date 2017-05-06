## Inter process communication

![](/assets/IPC.png)

### 1. Message passing IPC

![](/assets/message_passing_IPC.png)

pros: OS manages

cons: overheads \(copy data to channel and pass to database\)

### 2. Shared memory IPC

![](/assets/shared_memory_IPC.png)

pros: OS is out of the way

cons: cannot use OS APIs, reimplement the code

