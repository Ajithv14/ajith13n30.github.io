# useless
## Description
There's an interesting script in the user's home directory
The work computer is running SSH. We've been given a script which performs some basic calculations, explore the script and find a flag
>ssh into the instance with provided details.

hint:
```bash
# ssh guide
ssh -p port_number username@hostname
# While doing 'ls' found a script named 'useless'
ls
# After reading the script found that there is a manual page for this script

# invoke manual
man useless
```

<details>
<summary>Spoiler</summary>

picoCTF{us3l3ss_ch4ll3ng3_3xpl0it3d_5562}

</details>
