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


## Usage

### Interactive Mode

```bash
./battery_spoofer.sh
```

Menu Options:
- `s` — Set battery level  
- `r` — Reset battery state  
- `e` — Exit  


### Direct Commands

```bash
# Set battery level to 55%
./battery_spoofer.sh set 55

# Reset battery state
./battery_spoofer.sh reset
```


## Requirements

- Termux installed

### For Shizuku mode:
- `rish` binary must be in the same directory
- Make it executable: `chmod +x rish`
- Shizuku app must be running in the background

### For root mode:
- Device must be rooted
- `su` must be available in Termux


## Notes

- Automatically chooses root or shizuku mode
- Displays clear messages on failure (e.g., missing `rish`, Shizuku not running)
- Can work fully offline after setup


## License

MIT License


## Credits

Developed with care by:

- **MERBAH3266**
- **CHAOUCHI**
