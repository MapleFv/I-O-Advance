#  linux 

### lsof -p [port]

查看端口号对应的文件描述符分配情况

### netstat

查看网络连接命令

- -n  以数字形式显示地址和端口号

- -a 显示所有连接和侦听端口，TCP和UDP协议都会列出来，包括本地IP端口，远程IP和端口,以及连接状态

- t (tcp) 仅显示tcp相关选项

- -p 显示proto指定的协议的链接，proto可以是下列任何一个：TPC、UDP、TCPv6或UDPv6

### jps 

全称：java virtual machine process status tool 

列出本季所有java的pid

### strace

strace -ff -o out cmd

- -tt：在每行输出的前面，显示毫秒级别的时间
- -T：显示每次系统调用所花费的时间
- -v：对于某些相关调用，把完整的环境变量，文件 stat 结构等打出来。
- -f：跟踪目标进程，以及目标进程创建的所有子进程
- -e：控制要跟踪的事件和跟踪行为，比如指定要跟踪的系统调用名称
- -o：把 strace 的输出单独写到指定的文件
- -s：当系统调用的某个参数是字符串时，最多输出指定长度的内容，默认是 32 个字节
- -p：指定要跟踪的进程 pid，要同时跟踪多个 pid，重复多次 -p 选项即可。
- -ff：如果提供 -o FILENAME，则所有进程的跟踪结果输出到相应的 FILENAME.pid 中，pid 是各进程的进程号

# **04 C10K问题及NIO精讲和IO模型性能压测**



### 1 BIO阻塞，NIO不阻塞的理解

BIO代码 SocketOPropertites

![image-20230411144623033](https://cdn.jsdelivr.net/gh/MapleFv/BolgImgs/202304111446392.png)



NIO

![image-20230411150304182](https://cdn.jsdelivr.net/gh/MapleFv/BolgImgs/202304111503397.png)





# 05 网络编程之多路复用器及Epoll精讲

