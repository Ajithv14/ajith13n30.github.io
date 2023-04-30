# repetitions
## Description
Can you make sense of this file?
Download the file [here](https://artifacts.picoctf.net/c/475/enc_flag).

hint:
```bash
# download given file
wget https://artifacts.picoctf.net/c/475/enc_flag
# seems like the text in this file is base64 encoded.
# After decrypting found that it is encoded multiple times

```
>https://www.base64decode.org/ can use this url for decoding base64.

<details>
<summary>Spoiler</summary>

picoCTF{base64_n3st3d_dic0d!n8_d0wnl04d3d_492767d2}

</details>

## Bonus:
```bash
# cli tool for base64 encoding and decoding.
base64 --decode enc_flag|base64 --decode|base64 -d|base64 -d|base64 -d|base64 -d
```