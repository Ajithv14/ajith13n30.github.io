# Tab, Tab, Attack
## Description
Using tabcomplete in the Terminal will add years to your life, esp. when dealing with long rambling directory structures and filenames: [Addadshashanammu.zip](https://mercury.picoctf.net/static/fe16c756149cfa85f23e73cd9dbd6a25/Addadshashanammu.zip)

> Tab completion is a wonderful feature, which can be used in many ways like you don't have to always remember the file structure. You can move to a unknown folder and without using `ls` you can view the content of the folder.
>
> Tab completion: tap the tab key twice and see the magic.

hint:
```bash
# Download file provided
wget https://mercury.picoctf.net/static/fe16c756149cfa85f23e73cd9dbd6a25/Addadshashanammu.zip
# unzip it
unzip Addadshashanammu.zip
# Use tab after typing cd and go deep into the folder by using tab completion.
cd Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku
# check filetype
file fang-of-haynekhtnamet
# It is a binary file so we can try the string command
strings fang-of-haynekhtnamet | grep pico
```

<details>
<summary>Spoiler</summary>

picoCTF{l3v3l_up!_t4k3_4_r35t!_76266e38}

</details>
