# Network - Challenge 06

This challenge was an pcapng file.

Challenge ask for an ipv6 address that might be able to connect to internet.

Open pcapng file with wireshark. (Or you can convert pcapng file to pcap file and used networkminer)

After view overall pcap file, I found out that this was a cisco bgp rounter config traffic.

![image-20221003142942419](./network-challenge06.assets/image-20221003142942419.png)

![image-20221003143025044](./network-challenge06.assets/image-20221003143025044.png)

I google about how to config gateway and found some interesting information.

```
https://community.spiceworks.com/how_to/164102-configure-a-gateway-of-last-resort-or-default-route-on-cisco-routers
```

![image-20221003143335429](./network-challenge06.assets/image-20221003143335429.png)

Try search packet with keyword "Gateway of last resort"

![image-20221003143316543](./network-challenge06.assets/image-20221003143316543.png)

Found ip 122[.].57.1.121

Convert to ipv6 and answer.

```
https://iplocation.io/ipv4-to-ipv6/122.57.1.121
```

![image-20221003143540685](./network-challenge06.assets/image-20221003143540685.png)

```
::ffff:7a39:179
```

![image-20221003143549572](./network-challenge06.assets/image-20221003143549572.png)