
# RofiPeek

**RofiPeek** is a lightweight tool that overlays your keyboard layout on the screen using [Rofi](https://github.com/davatorium/rofi). It provides a simple way to display any keyboard layout as a text file, making it easy to visualize your layout.

## Prerequisites

Before using RofiPeek, ensure that you have the following installed:

- **Rofi**: A window switcher that RofiPeek uses to display the keyboard layout.
  
  You can install Rofi on most Linux distributions using the package manager. For example:
  ```bash
  sudo apt install rofi
  ```

## Installation

1. **Clone the Repository**:
   Begin by cloning the RofiPeek repository:
   ```bash
   git clone https://github.com/yourusername/rofipeek.git
   cd rofipeek
   ```

2. **Ensure Rofi is Installed**:
   Make sure that **Rofi** is installed on your system. Follow the installation instructions above if you don't have it yet.

## File Structure

The repository contains the following files and folders:

- **layouts/**: This folder contains different text files for various keyboard layouts.
- **rofipeek**: The main script that launches Rofi to display the keyboard layout.
- **rofipeek.rasi**: A theme file used by Rofi to customize the display style of the keyboard layout.

## Usage

To use RofiPeek, you need to run the `rofipeek` script with two arguments:

1. **Layout File**: A simple text file containing the keyboard layout.
2. **Theme File**: The `rofipeek.rasi` file that defines the theme and appearance for Rofi.

### Example Command

Run the following command to display a keyboard layout using the `rofipeek` script:

```bash
./rofipeek layouts/colemak-dh-block.txt rofipeek.rasi
```

## Keybinding Setup

To make RofiPeek easier to invoke, you can set up a keybinding in your window manager.

For example, in **i3**, add the following to your configuration file:

```bash
bindsym $mod+Shift+L exec --no-startup-id /path/to/rofipeek /path/to/keyboard_layout.txt /path/to/rofipeek.rasi
```

This will bind the key combination `$mod+Shift+L` to display the keyboard layout using RofiPeek.

## Customizing Keyboard Layouts

You can easily customize the layout by editing or adding new text files in the **layouts/** folder. Each layout file should be a simple text file with the arrangement of your keyboard's keys.

If you're unsure about how to create a keyboard layout, you can use a tool like **ChatGPT** to help generate the layout text file based on your preferences. Just describe the layout you need, and you can get the corresponding text file ready to use with RofiPeek.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Happy Learning !!
