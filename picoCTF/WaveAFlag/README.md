# Wave a flag
## Description
Can you invoke help flags for a tool or binary? [This program](https://mercury.picoctf.net/static/cfea736820f329083dab9558c3932ada/warm) has extraordinarily helpful information...

hint:
```bash
# Download file
wget https://mercury.picoctf.net/static/cfea736820f329083dab9558c3932ada/warm
#Check file type
file warm
# the above file seems to be a binary we can directly run it but generally we should not run a binary as it is since we don't know what it will do. For this challenge we can run the file
# add excecution permission
chmod +x warm
# run it with -h parameter to get help
./warm -h
```

<details>
<summary>Spoiler</summary>

picoCTF{b1scu1ts_4nd_gr4vy_30e77291}

</details>

## Bonus:

Without running the script we can extract the strings using ``` strings``` command.
```bash
strings warm|grep pico
```