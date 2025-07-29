# NKNet 🌐 - 南开大学校园网命令行工具

[[ENGLISH](README.md)] | [中文]

![version-2.1.0](https://img.shields.io/badge/version-2.1.0-blue)
![python->=3.6](https://img.shields.io/badge/python->=3.6-blue?logo=python&logoColor=white)
![GitHub License](https://img.shields.io/github/license/alumik/nknet)

一个简单的南开大学校园网认证管理命令行工具。通过自动凭据管理和状态检查，简化您的网络登录/注销流程。

## ✨ 功能特性

- 🔐 **安全认证** - 登录和注销校园网
- 💾 **凭据管理** - 自动保存和加载登录凭据
- 📊 **网络状态** - 实时网络连接检查，彩色输出
- ⚡ **快速轻量** - 最少依赖，最高效率

## 🚀 快速开始

### 安装

```bash
# 克隆仓库
git clone https://github.com/AlumiK/nknet.git
cd nknet

# 设置可执行权限 (Linux/macOS)
chmod +x nknet.py

# 安装依赖
pip install -r requirements.txt
```

### 基本用法

```bash
# 登录校园网
nknet login

# 检查网络状态
nknet status

# 注销校园网
nknet logout

# 使用保存的凭据自动登录
nknet login --auto-login

# 清除保存的凭据
nknet clear
```

## 📋 命令说明

### `login` - 连接到校园网

```bash
nknet login [选项]
```

**选项：**
- `-c, --config PATH` - 指定自定义配置文件路径
- `-a, --auto-login` - 使用保存的凭据自动登录

**示例：**
```bash
# 交互式登录（提示输入用户名/密码）
nknet login

# 使用保存的凭据自动登录
nknet login --auto-login

# 使用自定义配置文件
nknet login --config /path/to/config.json
```

### `status` - 检查网络状态

```bash
nknet status
```

显示当前网络连接状态：
- 🟢 **online** - 已连接到互联网
- 🔴 **offline** - 无互联网连接
- 当前已登录用户名（如果已登录）

### `logout` - 断开校园网连接

```bash
nknet logout
```

### `clear` - 清除保存的凭据

```bash
nknet clear [选项]
```

**选项：**
- `-c, --config PATH` - 指定自定义配置文件路径

## 🔒 安全提示

密码以简单加密形式存储在本地 - 请确保适当的文件权限设置。

## 🤝 贡献

欢迎贡献！请随时提交Pull Request。对于重大更改，请先创建issue讨论您想要更改的内容。

## 📝 许可证

本项目基于MIT许可证 - 详情请参阅 [LICENSE](LICENSE.md) 文件。

## 🐛 问题反馈与支持

如果您遇到任何问题或有疑问：

1. 查看现有的 [Issues](https://github.com/yourusername/nknet/issues)
2. 创建新的issue并提供详细信息
3. 请包含您的Python版本和操作系统信息

---

**为南开大学学生用❤️制作**

[报告Bug](https://github.com/AlumiK/nknet/issues) · [请求功能](https://github.com/AlumiK/nknet/issues) · [贡献代码](https://github.com/AlumiK/nknet/pulls)