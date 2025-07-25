# Battery Spoofer

A simple yet powerful battery spoofing tool for **Termux**.  
Supports both **root mode** and **Shizuku mode**.  
Allows setting or resetting the fake battery level with a clean interactive UI or via direct command arguments.


## Features

- Works in **Termux only**
- Supports **root** or **Shizuku** (auto-detection)
- Set fake battery level to any integer (even negative!)
- Reset battery state easily
- Built-in retry system
- Animated UI with colors and user-friendly messages


## Installation

Run this command directly in **Termux**:

```bash
bash <(curl -fsSL https://bit.ly/bspoof)
```

Follow the on-screen steps:

- On first install, you'll be asked to confirm by typing **`y`** to proceed.
- If the script is already installed, it will detect the existing version and ask whether to update.
- Press **`y`** then **Enter** to confirm the update.  
  Pressing **`n`** or any other key will **cancel the installation**.

After successful installation, run the tool using:

```bash
bspoof
```


## Usage

### Interactive Mode

```bash
~ $ bspoof
```

Menu Options:
- `s` — Set battery level  
- `r` — Reset battery state  
- `e` — Exit  


### Direct Commands

```bash
# Set battery level to 55%
~ $ bspoof set 55

# Reset battery state
~ $ bspoof reset
```


## Requirements

- Termux installed

### For Shizuku mode:
- `rish` script must be in the same directory
- Make it executable: `chmod +x rish`
- Shizuku app must be running in the background

### For root mode:
- Device must be rooted
- `su` must be available in Termux


## Notes

- Automatically chooses root or shizuku mode
- Can work fully offline after setup

> [!WARNING]
> This script is safe and has been tested under normal conditions.  
> However, we are **not responsible** for any unexpected behavior or damage that may occur.  
> Use it **at your own risk**.

## License

MIT License


## Credits

Developed with care by:

- [**MERBAH3266**](https://github.com/MERBAH3266)
- [**CHAOUCHI16**](https://github.com/CHAOUCHI16)
