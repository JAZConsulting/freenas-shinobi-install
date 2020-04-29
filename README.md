# freenas-shinobi-install
Taken directly from Reddit [here](https://www.reddit.com/r/ShinobiCCTV/comments/9sgzae/install_shinobi_on_freenas/). Thanks guys!

# Using this script
I didn't want to set up ssh into my jail, and I could not copy/past into the browser shell. With my jail having internet access (for now) I figured it would be easier to put this in a git and pull it into the jail. I was right!

```sh
root@your-jail# portsnap fetch extract
root@your-jail# portsnap update
root@your-jail# pkg update -f
root@your-jail# pkg install git 
```
Once you pull it, simply

 ```sh
 root@your-jail# chmod +x ./freenas-shinobi-install/shinobi-freenas-installer.csh
 root@your-jail# ./freenas-shinobi-install/shinobi-freenas-installer.csh
 ```
