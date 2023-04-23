# Nice netcat...
## Description
There is a nice program that you can talk to by using this command in a shell: $ nc mercury.picoctf.net 35652, but it doesn't speak English...

>netcat (often abbreviated to nc) is a computer networking utility for reading from and writing to network connections using TCP or UDP.


hint:
```bash
nc mercury.picoctf.net 35652
```
The dump you got was ASCII value use any online ascii converter to get flag.
https://www.duplichecker.com/ascii-to-text.php

<details>
<summary>Spoiler</summary>

picoCTF{g00d_k1tty!_n1c3_k1tty!_9b3b7392}

</details>

## Bonus:
```bash
nc mercury.picoctf.net 35652| awk '{printf("%c",$1)}' 
```