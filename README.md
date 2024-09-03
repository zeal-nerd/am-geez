# am-geez.mim - Custom Keybinding for IBus and ibus-m17n

This repository provides a custom Windows-like keybinding configuration for typing in Amharic (Ge'ez script) using the IBus input method framework and the `ibus-m17n` engine on Linux.
### Tested on:
  1. Debian 12
  2. PopOs -> based on Ubuntu
  3. EndeavourOS -> based on Arch linux

## What is IBus and ibus-m17n?

### IBus (Intelligent Input Bus)
IBus is a widely-used input method framework in Linux that enables users to type in multiple languages, especially those with complex scripts. It serves as a bridge between your keyboard input and the text displayed in your applications, handling the conversion of key presses into the appropriate characters or scripts.

### ibus-m17n
The `ibus-m17n` package integrates the powerful `m17n` library with IBus, allowing the use of a variety of pre-defined and custom input methods. The `m17n` library supports numerous languages and scripts, making it easier to type in languages like Amharic by mapping specific key sequences to the correct characters.

## Setup Instructions

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

### Step 4: Configure IBus
  1. Open IBus Preferences:
       - Open the IBus preferences window by running ibus-setup in your terminal or by navigating to the IBus Preferences from your system settings.
         
     
![Screenshot-- (2)](https://github.com/user-attachments/assets/99c087c5-3525-4018-bec3-09ffc3b39ecb)


  2. Add the Amharic (Ge'ez) Input Method:
      - In the ___Input Method___ tab, click the ___Add___ button.

![Screenshot --(3)](https://github.com/user-attachments/assets/cf36f40e-f0ff-4597-bc18-73995fcb3aac)

  - Select ___Amharic___ from the list, and choose the ___am-geez___ input method.

![Screenshot --(4)](https://github.com/user-attachments/assets/b3c93bea-7abf-479f-8256-6e30602a3d9d)


![Screenshot --(6)](https://github.com/user-attachments/assets/3aa1ac82-29fb-4104-8282-52e3d66cfbb3)


![Screenshot--- (7)](https://github.com/user-attachments/assets/20f35c68-cb71-4a04-8cd5-04ded32d7615)


  3. Set Up Custom Keyboard Shortcut:
       - In the ___General___ tab, you can customize the keyboard shortcut for switching input methods. Set this to your preferred Windows-like keybinding (e.g., `Alt + Shift`).
    

![Screenshot ---(2)](https://github.com/user-attachments/assets/1cf93e07-7e19-4cc0-95fe-a2f721164d3b)


![Screenshot----(5)](https://github.com/user-attachments/assets/bc645b1f-bd84-452c-b785-b1aa35fd5572)


### Step 5: Start Typing in Amharic

With everything configured, you can now switch between your input methods using the keyboard shortcut you set up. Select the Amharic (Ge'ez) input method and start typing in Amharic using your custom keybindings.


> #### Contributing
> 
> Feel free to fork this repository and make improvements or adjustments to the .mim file. Pull requests are welcome!
