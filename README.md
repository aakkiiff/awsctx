# 📦 `awsctx` — Simple AWS CLI Profile Manager

`awsctx` is a lightweight Bash utility that helps you manage multiple AWS CLI profiles. It supports:

- ➕ Adding new profiles
- 🔁 Switching the default profile
- 📋 Listing all profiles
- 🗑 Removing unwanted profiles
- 🆘 Helpful usage display

---
## ⚠️ Prerequisites

- [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)
- [`fzf`](https://github.com/junegunn/fzf): for interactive profile selection

Install `fzf` with:

```bash
sudo apt update && sudo apt install fzf -y
```

## 🚀 Installation

### 📂 1. Clone or download the script

```bash
git clone https://github.com/aakkiiff/awsctx.git
cd awsctx
```
### 🛠 2. Make it executable and install

```bash
chmod +x awsctx
sudo mv awsctx /usr/local/bin/
```

That's it! Now you can use `awsctx` from anywhere in your terminal.

---

## 📚 Usage

```bash
awsctx                    # Interactively switch AWS profile
awsctx add                # Add a new AWS profile
awsctx ls                 # List all AWS profiles
awsctx rm <profile_name>  # Remove a specific AWS profile
awsctx --help             # Show usage info
```

---

## 🧪 Example

```bash
awsctx add
# Enter profile name: my-dev
# AWS Access Key ID: AKIAxxxx
# AWS Secret Access Key: ****************
# Default region (optional): us-east-1
```

Then switch profiles:

```bash
awsctx
# (fzf menu shows profiles to select)
```

---

## 📦 Uninstall

```bash
sudo rm /usr/local/bin/awsctx
```