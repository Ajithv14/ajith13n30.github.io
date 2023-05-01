# HashingJobApp
AUTHOR: LT 'SYREAL' JONES
## Description
If you want to hash with the best, beat this test!
> nc saturn.picoctf.net 49697

hint:
```bash
nc saturn.picoctf.net 49697
```
> Use the below url to generate md5 hash online
>
>[md5 generator](https://gchq.github.io/CyberChef/#recipe=MD5())

You can also use linux cli tool `md5sum`
```bash
echo -n "Text"|md5sum
# Here -n is mandatory
```
<details>
<summary>Spoiler</summary>

picoCTF{4ppl1c4710n_r3c31v3d_3eb82b73}

</details>

## Bonus:
```python
import hashlib
while 1:
    word=input("ENter something to convert to md5 hash or CTRL+c to exit: ")
    print(hashlib.md5(word.encode()).hexdigest())
```
OR
```bash
python -c 'import hashlib;
while 1:
    word=input("ENter something to convert to md5 hash or CTRL+c to exit: ")
    print(hashlib.md5(word.encode()).hexdigest())'
```