# python Warngling
## Description
Python scripts are invoked kind of like programs in the Terminal... Can you run [this Python script](https://mercury.picoctf.net/static/b351a89e0bc6745b00716849105f87c6/ende.py) using [this password](https://mercury.picoctf.net/static/b351a89e0bc6745b00716849105f87c6/pw.txt) to get [the flag](https://mercury.picoctf.net/static/b351a89e0bc6745b00716849105f87c6/flag.txt.en)?

> ` python: ` A good language to do various stuffs like automation, scripting, frontend, backend, machine learning etc...

hint:
```bash
# en/de-coder script
$ wget https://mercury.picoctf.net/static/b351a89e0bc6745b00716849105f87c6/ende.py
# password file
$ wget https://mercury.picoctf.net/static/b351a89e0bc6745b00716849105f87c6/pw.txt
#encoded flag
$ wget https://mercury.picoctf.net/static/b351a89e0bc6745b00716849105f87c6/flag.txt.en
```
> for understanding the challenge read the python script by `less ende.py` from here we understand the way of encoding and decoding 

```bash
$ python ende.py --help        
Usage: ende.py (-e/-d) [file]
Examples:
  To decrypt a file named 'pole.txt', do: '$ python ende.py -d pole.txt'
# finally
python ende.py -d flag.txt.en
# add password found in pw.txt file "67c6cc9667c6cc9667c6cc9667c6cc96"
```

<details>
<summary>Spoiler</summary>

picoCTF{4p0110_1n_7h3_h0us3_67c6cc96}

</details>
