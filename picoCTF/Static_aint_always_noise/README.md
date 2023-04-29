# Static ain't always noise
## Description
Can you look at the data in this binary: [static](https://mercury.picoctf.net/static/7495259e963bd5b67d0fb8b616652618/static)? This [BASH script](https://mercury.picoctf.net/static/7495259e963bd5b67d0fb8b616652618/ltdis.sh) might help!

hint:
```bash
# Download static file
wget https://mercury.picoctf.net/static/7495259e963bd5b67d0fb8b616652618/static
# Download Bash Script
wget https://mercury.picoctf.net/static/7495259e963bd5b67d0fb8b616652618/ltdis.sh
#Check file type
file static
# the above file seems to be a binary we can directly run it but generally we should not run a binary as it is since we don't know what it will do. For this challenge we can run the file
# analyze ltdis.sh file
cat ltdis.sh
# the above file has the procedure to solve this
# dump all the objects of the static file
objdump -Dj .text static > static.ltdis.x86_64.txt
# gather strings found in the output of above file
strings -a -t x static.ltdis.x86_64.txt > static.ltdis.strings.txt
# grep the flag
cat static.ltdis.strings.txt | grep pico
```

<details>
<summary>Spoiler</summary>

picoCTF{d15a5m_t34s3r_f6c48608}

</details>

## Bonus:
Easy way

Without running the script we can extract the strings using ` strings` command.
```bash
strings static|grep pico
```