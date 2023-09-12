# PING 的工作原理？
- 用于测试网络连接和测量到目标主机的往返延迟RTT
- PING 基于网络层的 ICMP（Internet Control Message Protocol，互联网控制报文协议），其主要原理就是通过在网络上发送和接收 ICMP 报文实现的，包含差错、查询报文类型，PING 命令会向目标主机发送 ICMP Echo Request。
如果两个主机的连通性正常，目标主机会返回一个对应的 ICMP Echo Reply。
#DNS
# ARP
