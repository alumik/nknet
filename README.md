# NKNet 🌐 - Nankai University Campus Network CLI Tool (南开大学校园网命令行工具)

![version-2.0.2](https://img.shields.io/badge/version-2.0.2-blue)
![python->=3.6](https://img.shields.io/badge/python->=3.6-blue?logo=python&logoColor=white)
![GitHub License](https://img.shields.io/github/license/alumik/nknet)

A simple and elegant command-line tool for managing campus network authentication at Nankai University.
Streamline your network login/logout process with automatic credential management and status checking.

## ✨ Features

- 🔐 **Secure Authentication** - Login and logout from campus network
- 💾 **Credential Management** - Automatic saving and loading of login credentials
- 📊 **Network Status** - Real-time network connectivity checking with colored output
- ⚡ **Fast & Lightweight** - Minimal dependencies, maximum efficiency

## 🚀 Quick Start

### Installation

```bash
# Clone the repository
git clone https://github.com/AlumiK/nknet.git
cd nknet

# Make executable (Linux/macOS)
chmod +x nknet.py

# Install dependencies
pip install -r requirements.txt
```

### Basic Usage

```bash
# Login to campus network
nknet login

# Check network status
nknet status

# Logout from campus network
nknet logout

# Auto-login with saved credentials
nknet login --auto-login
```

## 📋 Commands

### `login` - Connect to Campus Network

```bash
nknet login [OPTIONS]
```

**Options:**
- `-c, --config PATH` - Specify custom config file path
- `-a, --auto-login` - Use saved credentials for automatic login
- `-n, --no-save` - Don't save credentials to config file

**Examples:**
```bash
# Interactive login (prompts for username/password)
nknet login

# Auto-login with saved credentials
nknet login --auto-login

# Login without saving credentials
nknet login --no-save

# Use custom config file
nknet login --config /path/to/config.json
```

### `status` - Check Network Status

```bash
nknet status
```

Displays current network connectivity status with:
- 🟢 **Online** - Connected to Internet
- 🔴 **Offline** - No Internet connection
- Current logged-in username (if authenticated)

### `logout` - Disconnect from Campus Network

```bash
nknet logout
```

Safely logs out from the campus network authentication system.

## 🔒 Security Notes

- Passwords are stored locally in plain text - ensure proper file permissions

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.

## 🐛 Issues & Support

If you encounter any issues or have questions:

1. Check existing [Issues](https://github.com/yourusername/nknet/issues)
2. Create a new issue with detailed information
3. Include your Python version and operating system

---

**Made with ❤️ for Nankai University students**

[Report Bug](https://github.com/AlumiK/nknet/issues) · [Request Feature](https://github.com/AlumiK/nknet/issues) · [Contribute](https://github.com/AlumiK/nknet/pulls)
