#  linux 

### lsof -p [port]

查看端口号对应的文件描述符分配情况

### netstat

查看网络连接命令

-n  以数字形式显示地址和端口号

-a 显示所有连接和侦听端口，TCP和UDP协议都会列出来，包括本地IP端口，远程IP和端口,以及连接状态

-t (tcp) 仅显示tcp相关选项

-p 显示proto指定的协议的链接，proto可以是下列任何一个：TPC、UDP、TCPv6或UDPv6

### jps 

全称：java virtual machine process status tool 

列出本季所有java的pid