## 🟦 Lists

Open your `hosts` file with `vim` and use `:/` to search for entries.

### Unified Hosts Lists

1. **Personal List** – My custom entries  
2. **Luke Smith’s List** – [GitHub Link](https://github.com/LukeSmithxyz/etc/blob/master/ips)  
3. **dan.me.uk’s TOR List** – [Website Link](https://www.dan.me.uk/torlist/?full) ❗ *TOR will no longer work after using this*  
4. **columndeeply’s List** – [GitHub Link](https://github.com/columndeeply/hosts)

## 🟩 Devices

### Linux

Append the content to your system hosts file:

```bash
sudo cat hosts >> /etc/hosts
```

### Windows

Manually place the domains into:

```
C:\Windows\System32\drivers\etc\hosts
```

### Android

1. Enable `USB debugging` and `Rooted debugging` on your device  
2. Install `adb` on your computer:

   ```bash
   sudo pacman -S adb
   ```

3. Connect the device and push your local hosts file:

   ```bash
   adb root
   adb remount
   adb push /etc/hosts /system/etc
   ```

### iPhone (irreversible)

1. Go to: `Settings > Screen Time > Communication Safety`  
2. Enable desired filters and blindly set a password  
3. ⚠️ This cannot be undone unless you call Apple Support

---

### 🟦 License

MIT License
