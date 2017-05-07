## Mutex

![](/assets/mutex.png)

#### Mutex API 

![](/assets/mutex_api.png)

#### Code Example

```
list<int> my_list;
Mutex m;
void safe_insert(int i){
    Lock(m){
        my_list.insert(i);
    } //unlock
}
```


