# Magikarp Ground Mission
## Description
Do you know how to move between directories and read files in the shell? Start the container, `ssh` to it, and then `ls` once connected to begin. Login via `ssh` as `ctf-player` with the password, `b60940ca`
Additional details will be available after launching your challenge instance.

hint:
```bash
# After launching ssh into the server 
ssh ctf-player@venus.picoctf.net -p 54980
# There are 3 pieces of flag in this challenge 1 of 3 flag is found in the login folder.
cat 1of3.flag.txt
# instructions for 2nd piece is found in the same folder itself.
cat instructions-to-2of3.txt
# As per instruction next piece of flag is in / folder.
cd /
cat 2of3.flag.txt
# instruction for 3rd piece of flag is in same / folder.
cat instructions-to-3of3.txt
# As per instruction 3rd flag is in home(~) folder.
cd ~
cat 3of3.flag.txt
```
<details>
<summary>Spoiler</summary>

picoCTF{xxsh_0ut_0f_\/\/4t3r_c1754242}

</details>