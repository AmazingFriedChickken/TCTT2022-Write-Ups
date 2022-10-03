# Network - Challenge 02

This challenge was an pcap file.

Open pcap file with NetworkMiner.

Found that attacker was trying to bruteforce a directory.

![image-20221003140122985](./network-challenge04.assets/image-20221003140122985.png)

![image-20221003140140549](./network-challenge04.assets/image-20221003140140549.png)

![image-20221003140155411](./network-challenge04.assets/image-20221003140155411.png)

If you use NetworkMiner like me. You can right click "open folder" to see all file from pcap dump.

![image-20221003140213158](./network-challenge04.assets/image-20221003140213158.png)

![image-20221003140230734](./network-challenge04.assets/image-20221003140230734.png)

Found secret.zip file

![image-20221003142436377](./network-challenge04.assets/image-20221003142436377.png)

This time zip file contain a lot of text file.

![image-20221003142518924](./network-challenge04.assets/image-20221003142518924.png)

To catch an SUS file, i trying to md5sum all file in directory.

```
md5sum *
```

![image-20221003142640976](./network-challenge04.assets/image-20221003142640976.png)

Found an imposter. file test_69.txt

```
Vm0weGQxTXdNVWRYV0d4VFYwZG9WMVl3WkZOVU1WcHpXa2M1VjAxWGVGWlZiVEZIVmpGYWMySkVUbGhoTVhCUVZteFZlRmRIVmtkaVIwWlRWakpvYjFaclpIcGxSbGw1Vkd0YWFGSnRVbGhVVkVGM1pVWmtXR1JIZEZOaVZscDZWVzAxUzJGV1NuTmpTRUpYWVRGYVNGUnJXbHBsUm1SMFVteHdWMDFFVmxwV1ZFb3dZVEZaZVZOcmFHaFRSVXBYV1ZkMFlWUkdXbGRYYlhScVRWZFNlbFl5TVRCVWJVcEhZMFJhVjJKVVFYaFdWRVpyVTBaS2NWZHNaR2xTTW1odlZtMXdUMkl5UmtkalJWcFlZbFZhV0ZSWGRHRlRiR1J5VjJ0MFZXSlZjRWhaTUZwM1ZqSkZlVlJZYUZaaGExcG9WakJhVDJNeVNrZFRiV3hvVFRCS1dWWXhaRFJpTVVWNVZtNU9WMWRIVWxsWldIQnpWMFpTVjJGRlRsTmlSbkJKVkZaU1UyRkdXbk5qUkVaV1ZqTm9WRlpxUm1GV01rNUhWRzFHVTFKV2NFVldiR1EwVVRGYVZrMVZWazVTUkVFNQ==
```

Decode with base64 9 times

![image-20221003142748622](./network-challenge04.assets/image-20221003142748622.png)