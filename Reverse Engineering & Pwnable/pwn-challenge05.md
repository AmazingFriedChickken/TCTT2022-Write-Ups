# Pwnable - Challenge 05

This challenge was an elf file.

Flag was stored on server.

Binary receive 2 user input as a short.

![image-20221003215311857](./pwn-challenge05.assets/image-20221003215311857.png)

short datatype has a range of -32768 to +32767

![Data_Types_in_C](./pwn-challenge05.assets/Data%252BTypes%252Bin%252BC%252BRivisited%252B2.jpg)

Look at this part of code.

```c
    local_a = local_e + local_c;
    if ((local_c < 0) || (local_e < 0)) {
      printf("\nME bad bad but still not good enough!\n",(ulong)(uint)(int)local_c,
             (ulong)(uint)(int)local_e,(ulong)(uint)(int)(short)local_a);
    }
    else if ((short)local_a < 0) {
      if (local_a == 0x8597) {
        putchar(10);
        printf("[*] The answer is %d",(ulong)(uint)(int)(short)local_a);
        system("cat SECRET.txt");
      }
      else {
        uVar1 = local_a;
        if ((short)local_a < 1) {
          uVar1 = -local_a;
        }
        printf("[*] The answer is %d\n",(ulong)uVar1);
      }
    }
```



First, it receive user input as local_e and local_c.

Then it store value of local_e add local_c in local_a.

```c
    local_a = local_e + local_c;
```

If user input 1 and 2 was lower then 0 it's will print error message

```c
    if ((local_c < 0) || (local_e < 0)) {
      printf("\nME bad bad but still not good enough!\n",(ulong)(uint)(int)local_c,
             (ulong)(uint)(int)local_e,(ulong)(uint)(int)(short)local_a);
    }
```

To get a flag, I must somehow send input 1 and input 2 that **Not lower then 0** and total **must be lower then zero** and value = -31337

![image-20221003220517597](./pwn-challenge05.assets/image-20221003220517597.png)

What happened when total was more then 32767 is it's become **minus**.

![image-20221003220908070](./pwn-challenge05.assets/image-20221003220908070.png)

![image-20221003221110975](./pwn-challenge05.assets/image-20221003221110975.png)

So i send first number as 32767 and second number as 1432 and got a flag

![Pasted image 20221001123307](./pwn-challenge05.assets/Pasted%20image%2020221001123307.png)

