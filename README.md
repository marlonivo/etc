## 🟦 Lists

My custom Block-List [19 entries]. Open your `hosts` file with `vim` and use `:/` to search for entries.

## 🟩 Devices

### Linux, MacOS

Append the content to your system hosts file:

```bash
sudo cat hosts >> /etc/hosts
```

### Windows

Manually place the domains into:

```
C:\Windows\System32\drivers\etc\hosts
```

### Android (rooted)

1. Enable `USB debugging` and `Rooted debugging` in developer settings.
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
3. ⚠️ This cannot be undone unless you call [Apple Support](https://support.apple.com/)

