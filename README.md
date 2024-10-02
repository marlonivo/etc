### 🟧 Installation & Update:

I have a `lazy-hosts` script for lazy humans and a quick chain-command to make use of it, it will:

1. Rewrite your `/etc/hosts` file.
2. Place a script in `/usr/bin` to autimatically update, when you do a system-wide-update.
3. Delete the `hosts` folder for you 
4. Dont forget to reboot afterwards

```
git clone https://github.com/marlonivo/hosts.git && cd hosts && chmod +x lazy-hosts && lazy-hosts　&& rm -r hosts
```

### 🟦 Blocklist:

When you use vim you can type `/`, to search for the individual parts:

1. **Personal Extras**: Add your own Stuff here
2. **Luke Smith's general-junk List**: [GitHub Link](https://github.com/LukeSmithxyz/etc/blob/master/ips) 
3. **dan.me.uk's tor-exit-node List**: [Website Link](https://www.dan.me.uk/torlist/?full) ❗ THIS WILL TOR BROWSER NOT ABLE TO CONNECT ANYMORE
4. **columndeeply 10 million-line-porn-block List**: [Github Link](https://github.com/columndeeply/hosts)


### 🟩 Devices:

#### Linux:
Assuming youre not lazy, dont use the `lazy-hosts` script, manually place the list in `/etc/hosts`, delete the folder and keep it updated yourself.

```bash
cd hosts && sudo cat hosts >> /etc/hosts && rm -r hosts
```

#### Windows:

Place the domains in `C:\Windows\System32\drivers\etc\hosts`.

#### Android :
1. Install `adb`:
   ```
   sudo pacman -S adb
   ```
2. Plug phone into your computer.
3. Run the following commands:
   ```
   adb root
   adb remount
   adb push /etc/hosts /system/etc
   ```

#### iPhone (irreversible workaround):
1. Go to `Settings > Screen Time > Communication Security`
2. Turn on filters for sensitive content and enter a password blindly.
3. This is a pretty good blocklist, you dont need to worry to stumple upon porn related content.

### 🟦 License: MIT
