# Termux - Android Terminal Emulator
**Termux** is a powerful terminal emulator for Android that brings the full capabilities of a Linux environment to your smartphone or tablet. No root access required!

## Table of Contents

- [What is Termux?](#-what-is-termux)
- [Features](#features)
- [Installation](#installation)
- [Getting Started](#getting-started)
- [Essential Commands](#essential-commands)
- [Package Management](#package-management)
- [Tutorial Videos](#tutorial-videos)
- [Documentation & Resources](#documentation--resources)
- [Community](#community)
- [FAQ](#faq)

## What is Termux?

Termux is a powerful terminal emulator and Linux environment for Android. It allows you to run a wide range of Linux packages, programming languages, and network tools, allowing you to:

- Run Linux commands on Android
- Install programming languages (Python, Node.js, Ruby, C/C++, etc.)
- Access device hardware and sensors
- Create automation scripts
- Run servers and development environments


## Features
### Core Capabilities
- **Full Linux Environment** - Complete terminal emulation with bash and zsh shells
- **Package Management** - Over 1000+ packages available via APT package manager
- **No Root Required** - Works on unrooted Android devices
- **Hardware Access** - Control camera, flashlight, sensors, and more via Termux:API
- **Multiple Sessions** - Run multiple terminal sessions simultaneously
- **Custom Styling** - Customize colors and fonts with Termux:Styling

### Development Environment
- **Programming Languages**: Python, Node.js, Ruby, C/C++, Go, Rust, Java
- **Text Editors**: Vim, Nano, Emacs
- **Version Control**: Git support
- **Web Development**: Local server hosting, PHP, HTML/CSS/JS
- **Database**: MySQL, SQLite support

### System Administration
- **SSH Client**: Connect to remote servers
- **File Management**: Complete file system access
- **Process Management**: Background tasks and job control
- **Network Tools**: Ping, wget, curl, netstat

## Installation
**Note**: You should use the F-Droid or GitHub version of Termux instead of the one on the Google Play Store. The Play Store version is often outdated, buggy, lacks functionality, and has previously been a source of security regressions and even a malicious, hijacked app. In contrast, F-Droid and GitHub versions are actively maintained, more stable, and generally considered safer.

### Watch this tutorial for installation: [Video](https://youtu.be/V1-zzo-tCyI)

#### F-Droid (Recommended)
```bash
# Download directly from F-Droid
https://f-droid.org/en/packages/com.termux/
```
- Most stable and up-to-date
- Regular security updates
- Community trusted

#### GitHub Releases
```bash
# Download latest release
https://github.com/termux/termux-app/releases
```
- Latest features
- Beta testing builds
- have experimental features

#### Google Play Store
```bash
# For Android 11+ devices
https://play.google.com/store/apps/details?id=com.termux
```
- Limited functionality
- Missing some features due to Play Store restrictions

**Note**: If you downloading termux from apk then The "unsafe app" warning may come for Termux due
to Google Play Protect flagging the F-Droid & Github version because it's built for older Android versions and may not have the latest privacy protections,While installing the APK, if unsafe app popup comes then click on read more and click on "Install anyway" to install Termux.


## System Requirements
- **Android Version**: 7.0+ (Android 5-6 limited support)
- **Architecture**: ARM, AArch64, i686, x86_64
- **Storage**: At least 300MB free space
- **RAM**: 1GB+ recommended

### Quick Setup:-
### First Steps

1. **Update System**
   ```bash
   pkg update && pkg upgrade
   ```

2. **Setup Storage Access**
   ```bash
   termux-setup-storage
   ```

## Essential Commands:-

### File Management
```bash
# Navigation
pwd                    # Show current directory
ls                     # List files and directories
ls -la                 # List with hidden files and details
cd <directory name>    # Change directory
cd ..                  # Go back one directory
cd ~                   # Go to home directory

# File Operations
mkdir <folder name>    # Create directory
rmdir <folder name>    # Remove empty directory
rm <file name>         # Delete file
rm -rf <folder name>   # Delete folder and contents
cp <source> <dest>     # Copy file
mv <old> <new>         # Move/rename file

# File Content
cat <file>             # Display file content
nano <file>            # Edit file with nano
vim <file>             # Edit file with vim
touch <file>           # Create empty file
grep <pattern> <file>  # Search text in file
```

### System Commands
```bash
# System Information
whoami                 # Current username
uname -a              # System information
uptime                # System uptime
free -h               # Memory usage
df -h                 # Disk usage
ps                    # Running processes
top                   # Process monitor
history               # Command history

# Network
ping <host>           # Test connectivity
wget <url>            # Download file
curl <url>            # HTTP requests
ifconfig              # Network interfaces
netstat               # Network connections
```

## Package Management

### PKG Commands (Recommended)
```bash
# Update and Upgrade
pkg update                 # Update package lists
pkg upgrade                # Upgrade installed packages
pkg update && pkg upgrade  # Update and upgrade together

# Install and Remove
pkg install <package>      # Install package
pkg uninstall <package>    # Remove package  
pkg reinstall <package>    # Reinstall package
pkg show <package>         # Show package info
pkg search <query>         # Search packages

# Package Information
pkg list-all               # List all available packages
pkg list-installed         # List installed packages
pkg files <package>        # Show files installed by package

# Cleanup
pkg clean                  # Clean package cache
pkg autoclean              # Remove outdated packages
```

### Popular Packages
```bash
# Development Tools
pkg install python git nodejs ruby golang
pkg install vim nano emacs
pkg install gcc clang make cmake

# Network Tools
pkg install openssh curl wget rsync
pkg install nmap wireshark-cli

# System Utilities
pkg install htop tree file which
pkg install tar zip unzip

# Web Development
pkg install apache2 nginx php mariadb
```

## Tutorial Videos

### Comprehensive Guides

1. **[Learn Termux In One Video (49 mins)](https://www.youtube.com/watch?v=PPurMircqsc)**
   - Complete beginner to advanced guide
   - Programming, web development, scripting
   - Covers Python, Java, C/C++, PHP, Node.js

2. **[Complete Termux Linux Tutorial 2025 (37 mins)](https://www.youtube.com/watch?v=4r5PM2avLqg)**
   - Installation to advanced usage
   - Linux commands and Python scripting
   - HTTP requests and automation

3. **[Termux Linux Commands FULL Tutorial (12 mins)](https://www.youtube.com/watch?v=VvQhT0e_58Q)**
   - Essential Linux commands
   - File operations and management
   - Perfect for beginners

4. **[Termux for Beginners | Simplilearn (10 mins)](https://www.youtube.com/watch?v=ulLjGFwFqbs)**
   - What is Termux and features
   - Installation and package management
   - Command cheat sheet

###  Learning Path
- Start with basic installation and setup videos
- Learn essential Linux commands
- Progress to programming and development
- Explore advanced topics like automation and networking

## Documentation & Resources

### Official Documentation
- **[Termux Wiki](https://wiki.termux.com)** - Comprehensive documentation
- **[Termux GitHub](https://github.com/termux/termux-app)** - Source code and issues
- **[Termux Packages](https://github.com/termux/termux-packages)** - Package repository
- **[Package Management Guide](https://wiki.termux.com/wiki/Package_Management)** - Detailed package info

### Useful Websites
- **[EasyMux](https://www.easymux.in/)** - Termux tutorials and downloads
- **[LearnTermux](https://www.learntermux.tech/)** - Commands and tutorials
- **[Termux Commands](https://www.termuxcommands.com/)** - Command reference

### Command Cheat Sheets
- **[Termux Command Cheat Sheet](https://denizhalil.com/2024/01/02/termux-commands-cheat-sheet/)** - Comprehensive command list
- **[Basic Commands PDF](https://www.learntermux.tech/2020/01/basic-commands-in-termux.html)** - Downloadable reference

## Community

### Get Help & Share
- **[Reddit r/termux](https://www.reddit.com/r/termux/)** - Active community discussions
- **[GitHub Issues](https://github.com/termux/termux-app/issues)** - Bug reports and feature requests
- **[Termux Community Guidelines](https://termux.dev/community)** - Community rules and guidelines

### Contributing
- Report bugs on GitHub
- Contribute to documentation
- Create and share packages
- Help other users in community forums

## FAQ

### Common Questions

**Q: Does Termux require root access?**
A: No, Termux works on unrooted devices. However, root access can unlock additional features.

**Q: Can I run GUI applications?**
A: Yes, using VNC server and desktop environments like XFCE or LXDE.

**Q: Is Termux safe for ethical hacking?**
A: Yes, but only use for learning and authorized testing. Respect legal boundaries.

**Q: Can I develop mobile apps with Termux?**
A: Yes, you can develop web apps, React Native apps, and use various development frameworks.

**Q: How much storage does Termux need?**
A: Base installation is ~180MB, but can grow with packages. 1GB+ recommended for development.

**Q: Can I run Termux on older Android versions?**
A: Limited support for Android 5-6. Android 7+ recommended for full functionality.

**Made with ❤️ by the Termux Community**

*Happy Terminal Hacking!*
