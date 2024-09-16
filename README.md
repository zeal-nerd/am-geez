# ⌨️ am-geez - Custom Keybinding for Linux Using IBus and ibus-m17n

This repository provides a custom phonetic Windows-like keybinding configuration for typing in Amharic (Ge'ez script) using the IBus input method framework and the `ibus-m17n` engine on Linux. 🚀

This configuration is designed to closely match the sounds of Amharic characters, making typing easier. While not all sounds are an exact match, the phonetic approach helps create a more intuitive way to input characters

### ✅ Tested on:

- Debian 12
- PopOs -> based on Ubuntu
- EndeavourOS -> based on Arch linux
- KalLinux -> based on Debian

## What is IBus and ibus-m17n? 🤔

### IBus (Intelligent Input Bus)

IBus is a widely-used input method framework in Linux that enables users to type in multiple languages, especially those with complex scripts. It serves as a bridge between your keyboard input and the text displayed in your applications, handling the conversion of key presses into the appropriate characters or scripts.

> **💡 Note:** While IBus is popular, it's not the only input method framework for Linux/Unix systems. There are others like Fcitx and UIM, which are lighter but harder to configure. This configuration can be used with any of these frameworks that support m17n settings.

### ibus-m17n

`ibus-m17n` integrates the powerful m17n library with IBus, supporting many languages and scripts. It makes typing in languages like Amharic a breeze by mapping key sequences to the correct characters.

## 🛠️ Setup Instructions

### Step 1: Install IBus and ibus-m17n

If you haven't already installed IBus and `ibus-m17n`, you can do so using your package manager. For example, on Debian-based systems:

```bash
sudo apt-get install ibus ibus-m17n
```

### Step 2: Copy the Custom .mim File

Clone this repository and copy the am-geez.mim file to the appropriate directory:

```bash
git clone https://github.com/zeal-nerd/am-geez.git
cd am-geez
sudo cp am-geez.mim /usr/share/m17n/
```

### Step 3: Restart or Reload IBus

After copying the .mim file, you need to restart or reload the IBus service for the changes to take effect:

```
ibus restart
```

Or if that doesn't work:

```
ibus-daemon -drx
```

### Step 4: Configure IBus 🛠️

1. Open IBus Preferences:
   - Open the IBus preferences window by running ibus-setup in your terminal or by navigating to the IBus Preferences from your system settings.

![Screenshot-- (2)](https://github.com/user-attachments/assets/99c087c5-3525-4018-bec3-09ffc3b39ecb)

2. Add the Amharic (Ge'ez) Input Method:
   - In the **_Input Method_** tab, click the **_Add_** button.

![Screenshot --(3)](https://github.com/user-attachments/assets/cf36f40e-f0ff-4597-bc18-73995fcb3aac)

- Select **_Amharic_** from the list, and choose the **_am-geez_** input method.

![Screenshot --(4)](https://github.com/user-attachments/assets/b3c93bea-7abf-479f-8256-6e30602a3d9d)

![Screenshot --(6)](https://github.com/user-attachments/assets/3aa1ac82-29fb-4104-8282-52e3d66cfbb3)

![Screenshot--- (7)](https://github.com/user-attachments/assets/20f35c68-cb71-4a04-8cd5-04ded32d7615)

3. Set Up Custom Keyboard Shortcut:
   - In the **_General_** tab, you can customize the keyboard shortcut for switching input methods. Set this to your preferred Windows-like keybinding (e.g., `Alt + Shift`).

![Screenshot ---(2)](https://github.com/user-attachments/assets/1cf93e07-7e19-4cc0-95fe-a2f721164d3b)

![Screenshot----(5)](https://github.com/user-attachments/assets/bc645b1f-bd84-452c-b785-b1aa35fd5572)

### Step 5: Start Typing in Amharic 🎉

With everything configured, you can now switch between your input methods using the keyboard shortcut you set up. Select the Amharic (Ge'ez) input method and start typing in Amharic using your custom keybindings.

> ### 💡 Contributing
>
> Feel free to fork this repository and make improvements or adjustments to the .mim file. Pull requests are welcome!

**Typing Amharic characters has never been easier on Linux. 🙌**

### 📧 Contact Me:

Email: zeal.nerd.kb@gmail.com
