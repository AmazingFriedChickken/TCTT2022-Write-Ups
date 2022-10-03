# Network - Challenge 01

This challenge was an pcap file.

Open pcap file with NetworkMiner.

Found a password protected zip file.

![image-20221003135433600](./network-challenge01.assets/image-20221003135433600.png)

![image-20221003135510015](./network-challenge01.assets/image-20221003135510015.png)

Trying to bruteforce a zip password and regret 5 second later.

```
fcrackzip secret.zip -u -D -p rockyou.txt
```

![image-20221003135811195](./network-challenge01.assets/image-20221003135811195.png)

 (╯°□°)╯︵ ┻━┻

![image-20221003135849265](./network-challenge01.assets/image-20221003135849265.png)



