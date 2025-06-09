# RecoveryDrive Reverse Engineer 🛠️

Welcome to **RecoveryDrive Reverse Engineer**! 🚀 This open-source project reimagines the Windows `recoveryDrive.exe` utility, empowering you to create recovery drives that not only restore your system but also recover your precious files. By reverse engineering the original tool, we’ve built a powerful, user-friendly alternative that’s free for everyone to use and explore. 🌟

[Download the executable now](https://github.com/Sk16er/RecoveryDrive/releases/download/EXE/RecoveryDrive.exe) and start protecting your data, or dive into the source code to see how it works! 🔍

## Table of Contents
- [What is This Project?](#what-is-this-project)
- [Why Reverse Engineer?](#why-reverse-engineer)
- [Features](#features-)
- [How to Use](#how-to-use-)
  - [Creating a Recovery Drive](#creating-a-recovery-drive)
  - [Recovering Files](#recovering-files)
- [For Curious Developers](#for-curious-developers-)
- [Troubleshooting](#troubleshooting-)
- [Limitations](#limitations-)
- [Contributing](#contributing-)
- [License](#license-)
- [Contact](#contact-)
- [Links](#links-)

## What is This Project? 🤔

The Windows `recoveryDrive.exe` is a built-in tool that creates USB recovery drives to reinstall Windows or fix system issues, like startup failures. However, it has a big drawback: it doesn’t include your personal files, leaving your documents, photos, and more at risk. 😕

This project reverse engineers `recoveryDrive.exe` to create an **open-source version** that:
- Builds recovery drives with your selected files included.
- Enables file recovery during system restoration.
- Offers transparency for developers to explore and improve.

Check out the official [Microsoft Support - Recovery Drive](https://support.microsoft.com/en-us/windows/recovery-drive-abb4691b-5324-6d4a-8766-73fab304c246) page for details on the original tool.

## Why Reverse Engineer? 🔧

Reverse engineering `recoveryDrive.exe` lets us:
- Understand how Windows creates recovery drives.
- Add file backup and recovery features missing in the original.
- Share an open-source solution that anyone can use or modify.

By making the code open, we invite the community to contribute, improve, and customize this tool for better data protection. 💾

## Features ✨

- **Custom Recovery Drives**: Create USB recovery drives that include your personal files.
- **File Recovery**: Retrieve your data during or after system restoration.
- **Open Source**: Explore the source code to understand the reverse engineering magic.
- **User-Friendly Executable**: Download and run [RecoveryDrive.exe](https://github.com/Sk16er/RecoveryDrive/releases/download/EXE/RecoveryDrive.exe) with no coding required.
- **Windows Compatibility**: Works on Windows 10 and 11.

## How to Use 🖱️

### Creating a Recovery Drive

1. **Download the Executable**:
   - Grab the latest `RecoveryDrive.exe` from the [Releases page](https://github.com/Sk16er/RecoveryDrive/releases/download/EXE/RecoveryDrive.exe).

2. **Prepare a USB Drive**:
   - Connect a USB drive with at least 16 GB of free space (32-64 GB recommended for larger backups).
   - **Note**: The drive will be formatted, so back up any existing data.

3. **Run the Tool**:
   - Double-click `RecoveryDrive.exe`.
   - Follow the prompts to select your USB drive and choose folders to include (e.g., Documents, Photos).
   - The tool will create a recovery drive with system files and your selected data.

4. **Safely Eject**:
   - Once complete, safely remove the USB drive and store it securely.

### Recovering Files

1. **Boot from the Recovery Drive**:
   - Insert the USB drive, restart your PC, and boot from the USB (adjust BIOS/UEFI settings if needed; see [Microsoft’s guide](https://support.microsoft.com/en-us/windows/change-the-boot-order-in-windows-10-4e4d31b5-7b0b-4e88-b46a-2a1c4f5e8e8b)).

2. **Access the Recovery Environment**:
   - In the Windows Recovery Environment (WinRE), select the option to recover files (prompts will guide you).

3. **Retrieve Your Files**:
   - Follow the on-screen instructions to copy files to a specified location (e.g., an external drive or restored system).

## For Curious Developers 🧑‍💻

Want to know how this works under the hood? The source code is open for you to explore! 📂

- **Reverse Engineering Details**: The project analyzes `recoveryDrive.exe` to understand its file structure and system recovery process. It then modifies the process to include user files and enable recovery in WinRE.
- **Source Code**: Check out the [repository](https://github.com/Sk16er/RecoveryDrive) and explore directories like `rc_20250610002018` for specific builds or configurations.
- **Get Involved**: Fork the repo, tweak the code, or suggest improvements via [Issues](https://github.com/Sk16er/RecoveryDrive/issues).

## Troubleshooting 🛠️

| **Issue** | **Solution** |
|-----------|--------------|
| **USB drive not detected** | Ensure the USB has 16+ GB free and try a different port or drive. |
| **Executable won’t run** | Right-click `RecoveryDrive.exe` and select “Run as administrator.” |
| **Files not included** | Verify you selected the correct folders during drive creation. |
| **Boot issues** | Check BIOS/UEFI settings to ensure USB boot priority (see [Microsoft’s boot guide](https://support.microsoft.com/en-us/windows/change-the-boot-order-in-windows-10-4e4d31b5-7b0b-4e88-b46a-2a1c4f5e8e8b)). |

## Limitations ⚠️

- **Windows Only**: Compatible with Windows 10 and 11; not tested on older versions.
- **USB Size**: Requires at least 16 GB, with more space needed for large file backups.
- **File Recovery Scope**: Only files included during drive creation can be recovered.
- **Technical Setup**: Booting from USB may require BIOS/UEFI adjustments.

## Contributing 🤝

Love open source? Join us! 🌍
1. Fork the [repository](https://github.com/Sk16er/RecoveryDrive).
2. Create a branch for your changes (`git checkout -b feature/awesome-improvement`).
3. Submit a pull request via [Pull Requests](https://github.com/Sk16er/RecoveryDrive/pulls).

Open an issue first for major changes or discussions.

## License 📜

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact 📬

Got questions or ideas? Open an issue on the [GitHub Issues](https://github.com/Sk16er/RecoveryDrive/issues) page or join the discussion!

## Links 🔗

- [GitHub Repository](https://github.com/Sk16er/RecoveryDrive)
- [Download RecoveryDrive.exe](https://github.com/Sk16er/RecoveryDrive/releases/download/EXE/RecoveryDrive.exe)
- [Issues](https://github.com/Sk16er/RecoveryDrive/issues)
- [Pull Requests](https://github.com/Sk16er/RecoveryDrive/pulls)
- [Microsoft Support - Recovery Drive](https://support.microsoft.com/en-us/windows/recovery-drive-abb4691b-5324-6d4a-8766-73fab304c246)
- [ZDNET - Windows Recovery Drive Guide](https://www.zdnet.com/article/how-to-create-a-windows-recovery-drive-in-4-easy-steps-before-its-too-late/)
- [Fileinspect - RecoveryDrive.exe Details](https://www.fileinspect.com/fileinfo/recoverydrive-exe/)

---

*Built with 💖 by Sk16er to make data recovery open and accessible for all!*