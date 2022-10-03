# Forensic - Challenge 06

This challenge was an windows xp ova file.

![image-20221003171512342](./forensic-challenge06.assets/image-20221003171512342.png)

First you need to extract a disk image file for an disk forensic tools.

I used Autopsy to solve this challenge. Which support only vmdk format.

https://www.autopsy.com/download/

So i import ova into vmware workstation and copy a vmdk for next step.

![image-20221003171953033](./forensic-challenge06.assets/image-20221003171953033.png)

![image-20221003151116300](./forensic-challenge06.assets/image-20221003151116300.png)

Select Data Source as Disk Image or VM File

![image-20221003151134570](./forensic-challenge06.assets/image-20221003151134570.png)

![image-20221003151155646](./forensic-challenge06.assets/image-20221003151155646.png)

![image-20221003151236116](./forensic-challenge06.assets/image-20221003151236116.png)

After imported data source. Wait for Autopsy to Analyzing file for a bit.

Search for a flag by click top right menu "Keyword Search".

![image-20221003164015121](./forensic-challenge06.assets/image-20221003164015121.png)

Found flag in file "hackernote.txt".

![image-20221003163951127](./forensic-challenge06.assets/image-20221003163951127.png)

---

## Extras

Found some interesting flag that not in this compitition too :)

![image-20221003163804446](./forensic-challenge06.assets/image-20221003163804446.png)