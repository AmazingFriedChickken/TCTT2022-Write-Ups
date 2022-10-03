# Mobile - Challenge 06

This challenge was an apk file.

Decompile an apk file with jadx-gui.

Found some regex in source code.

![image-20221003134224824](./mobile-challenge06.assets/image-20221003134224824.png)

Notice that line 68 was reference for a strings name large_text

![image-20221003134250412](./mobile-challenge06.assets/image-20221003134250412.png)

Found a very large text.

![image-20221003134345623](./mobile-challenge06.assets/image-20221003134345623.png)

Trying to mimic a code behavior, by use regex to extract a text.

REGEX

```
\.(\w)\.
```

![image-20221003134649171](./mobile-challenge06.assets/image-20221003134649171.png)

```
Z3BnZzIwMjJ7dDM3NzFhVF83MENfNTNQZTM3X3NlMHpfYTA3VTFBdDJ9
```

Found a base64 format text.

![image-20221003134718460](./mobile-challenge06.assets/image-20221003134718460.png)

Decoded

```
gpgg2022{t3771aT_70C_53Pe37_se0z_a07U1At2}
```

Notice that output has number and curly bracket. Try to shift a charactor by using ceasar chiper (ROT13)

![image-20221003134734966](./mobile-challenge06.assets/image-20221003134734966.png)



