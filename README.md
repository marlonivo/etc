### 🟧 Installation & Update

If youre a lazy-linuxer, use this command:

```
git clone https://github.com/marlonivo/hosts.git 
sh ./lazy-hosts.sh
```

1. `git clone https://github.com/marlonivo/hosts.git` - Downloads repo
2. `cd hosts && chmod +x lazy-hosts && lazy-hosts` - Uses this script to:
   1. Overwrite your `/etc/hosts`
   2. Puts itself to `/usr/bin` 
   3. Every update it will merge repos and keep `/etc/hosts` clean (no comments/empty lines)
3. `rm -r hosts` - Deletes repo from $HOME
4. Dont forget to reboot

-----

### 🟦 Lists

Open `/etc/hosts` with vim and press `:/` to search for:

1. **Personal List**: Your stuff
2. **Luke Smith's List**: [Link](https://github.com/LukeSmithxyz/etc/blob/master/ips) 
3. **dan.me.uk's List**: [Link](https://www.dan.me.uk/torlist/?full) ❗TOR WILL NOT CONNECT ANYMORE
4. **columndeeply's List**: [Link](https://github.com/columndeeply/hosts)

-----

### 🟩 Devices

#### Linux:
Transfer the content to your local hosts file.
```bash
sudo cat hosts >> /etc/hosts
```

#### Windows

Place the domains in `C:\Windows\System32\drivers\etc\hosts`.

#### Android
1. Activate `USB debugging` and `Rooted debugging` on your device.
2. Install `adb`, on your computer.

   ```
   sudo pacman -S adb
   ```
3. Plug device into computer.
4. Push your local host file to it.
   ```
   adb root
   adb remount
   adb push /etc/hosts /system/etc
   ```

#### iPhone (irreversible)
1. Go to `Settings > Screen Time > Communication Security`
2. Turn on the `filters of your choice` and enter a password blindly.
3. This can't be changed unless you call apple's service center.

### 🟦 License: MIT
