### Update Blocklist:
The script in `sync-hosts` can be used to update the Blocklist, just type in the terminal:
```
sync-hosts
```

### Blocklist Includes:
1. **Personal Extras**
2. **Luke Smith's General Junk List**: [GitHub Link](https://github.com/LukeSmithxyz/etc/blob/master/ips)
3. **dan.me.uk's Tor Exit Node List**: [dan.me.uk Link](https://www.dan.me.uk/torlist/?full) ❗ THIS WILL MAKE YOUR TOR BROWSER NOT ABLE TO CONNECT ANYMORE IN ORDER TO PREVENT SURROUNDING THE BLOCKLIST
4. **columndeeply 10 Million Porn List**: [Github Link](https://github.com/columndeeply/hosts)


### Where to Place the Domains:

#### Linux:
Place the domains in `/etc/hosts`:
```bash
sudo /etc/hosts
```

#### Windows (with administrator privileges):
Place the domains in `C:\Windows\System32\drivers\etc\hosts`.

##### Android (Developer tools and USB debugging must be turned on):
1. Install `adb`:
   ```
   sudo pacman -S adb
   ```
2. Plug the phone into the laptop.
3. Run the following commands:
   ```
   adb root
   adb remount
   adb push /etc/hosts /system/etc
   ```

##### iPhone (Irreversible):
1. Go to `Settings > Screen Time > Communication Security`.
2. Turn on filters for sensitive content and enter a password blindly.

