# Mobile - Challenge 06

This challenge was an apk file.

Decompile an apk file with jadx-gui.

![image-20221003123457269](./mobile-challenge01.assets/image-20221003123457269.png)

Found secret in base64 format.

```
private String secret = "==========gC9djTz0WTwM2XuFDTw4WdwY2XzI0X3gWOx02X1kjbxg0N7JjMwIDd0NGd==========";
```

Try to decode with base64.

![image-20221003173711823](./mobile-challenge01.assets/image-20221003173711823.png)

Try to reverse a strings and successfully decoded a flag.

![image-20221003123835339](./mobile-challenge01.assets/image-20221003123835339.png)