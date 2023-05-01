# Glitch Cat
AUTHOR: LT 'SYREAL' JONES
## Description
Our flag printing service has started glitching!
>$ nc saturn.picoctf.net 50561

hint:
```bash
nc saturn.picoctf.net 50561
```

<details>
<summary>Spoiler</summary>

picoCTF{gl17ch_m3_n07_9c42a45d}

</details>

## Bonus
```bash
# Paste the output from server like below
python3 -c "print('picoCTF{gl17ch_m3_n07_' + chr(0x39) + chr(0x63) + chr(0x34) + chr(0x32) + chr(0x61) + chr(0x34) + chr(0x35) + chr(0x64) + '}')"
```