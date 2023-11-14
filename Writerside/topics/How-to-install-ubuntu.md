# Setup Ubuntu Environment

In this section, we'll walk you through the process of setting up your development environment on Ubuntu. 
From installing key software components to configuring system settings, 
this guide ensures a smooth and efficient setup tailored to your coding needs. 
Whether you're a beginner or an experienced user, 
follow along to optimize your Ubuntu environment for a seamless and productive development experience.

> **Highlight important information**
>
> You can change the element to *tip* or *warning* by renaming the style attribute below.
>
{style="note"}

## Install Ubuntu OS

1. Obtain the Ubuntu image by visiting the [official website](https://ubuntu.com/download/desktop). 
You have the flexibility to either directly download the image or explore alternative download options tailored to your preferences.

2. Create a bootable usb drive 
   * [Create a bootable USB stick with Rufus on Windows](https://ubuntu.com/tutorials/create-a-usb-stick-on-windows)
   * [Create a bootable USB stick on Ubuntu](https://ubuntu.com/tutorials/create-a-usb-stick-on-ubuntu)
   * [Create a bootable USB stick on macOS](https://ubuntu.com/tutorials/create-a-usb-stick-on-macos)

3. Start by booting using the usb drive and follow those steps
   
4. choose `Try or Install Ubuntu` and click enter

   ![install](install_001.webp)

   ![install](install_002.webp)

5. choose your language then click on `Install Ubuntu`     

   ![install](install_003.webp)

   ![install](install_004.webp)

   ![install](install_005.webp)
   
   ![install](install_006.webp)
   
   ![install](install_007.webp)

   ![install](install_008.webp)

   ![install](install_009.webp)

   ![install](install_010.webp)

   ![install](install_011.webp)

   ![install](install_012.webp)

6. Remove the bootable USB and press `Enter`

   ![install](install_013.webp)

7. Now `Ubuntu` will boot

   ![install](install_014.webp)

   ![install](install_015.webp)

8. Enter the password set during the setup

   ![install](install_016.webp)

9. Now follow this steps 

   ![install](install_017.webp)

   ![install](install_018.webp)

   ![install](install_019.webp)

   ![install](install_020.webp)

   ![install](install_021.webp)

10. Occasionally new installation require update to the latest release. 
if not, you can find `Software Updater` in the `Application Menu` to launch the update

   ![install](install_022.webp)

   ![install](install_023.webp)

   ![install](install_024.webp)

11. Now restart the OS to start setting up or environment.

   ![install](install_025.webp)

## Setup Your development Environment 

As the cornerstone of my development, I've consistently employed Java, 
Go, and Python as my primary stack. 
This guide will provide step-by-step instructions for setting up these stacks. 
We'll commence with the installation of the most commonly used tools shared across all three programming languages.

1. Install commonly used tools, start terminal using `Ctrl + Alt + t` or from `Application Menu` 

   ```Bash
   sudo apt update -y && sudo apt upgrade -y
   sudo apt install build-essential manpages-dev -y 
   sudo apt install curl unzip git ffmpeg make -y
   ```
   
   ![install](tools_001.webp)

2. Git Config

   ```Bash
   git config --global user.name "Your Name"
   git config --global user.email your@email.com
   ```

   > **Git multiple git account**
   >
   > TO-DO adding multi account github.
   >
   {style="note"}

3. Now lets flavour our terminal to more powerful and nicer terminal

   - We will start by installing zsh terminal

     ```Bash
     sudo apt install zsh -y
     ```

   - Now lets change the default terminal to be `zsh`,
   to get the default terminal use the following command

     ```Bash
     echo $0
     ```
   
   - To change the default terminal to `zsh` use the following command

     ```Bash
     chsh -s $(which zsh)
     ```
   
   - Now reboot your OS

     ```Bash
     sudo reboot now
     ```

   - After the reboot open the terminal again you will find a message, 
   requires your action for configuration function for new user.
   press 2 to start the configuration, then you can validate the terminal using the same command as above.

     ![install](tools_005.webp)

     ![install](tools_006.webp)

   - Now lets install `oh my zsh`, open your browser head to this [link](https://ohmyz.sh/#install), 
   or copy the command and paste in the terminal.

     ```Bash
     sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
     ```

   - Now lets install `powerlevel10k` but first we need to install the recommended fonts. 
   In order to do so please download these artifacts [here](https://github.com/ramezhanna/my-dev-env-setup/blob/2145324bcb9e1a8d99cc85f30f68c1b54cadeac5/powerline-fonts.tar.xz).
   
   
   - 
5. hello

3. Step with a list.
   - List item
   - List item
   - List item