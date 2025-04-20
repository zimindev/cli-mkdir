# 📁 mkdir — Create Directories from the Command Line

The `mkdir` (make directory) command is used to create new directories in Linux and Unix-based systems. It's a simple but powerful tool when working with file systems in the terminal.

---

## ✅ Features

- Create single or multiple directories
- Set directory permissions on creation
- Automatically create nested (parent) directories
- Can be used in scripts for automated folder setup

---

## 🔧 Syntax

```bash
mkdir [OPTIONS] DIRECTORY_NAME
```

---

## 🚀 Basic Usage

### 📁 Create a Single Directory
```bash
mkdir my_folder
```

### 📁 Create Multiple Directories at Once
```bash
mkdir folder1 folder2 folder3
```

---

## 🧱 Create Nested Directories

### Create a directory with parent folders:
```bash
mkdir -p parent/child/grandchild
```

- `-p` creates any missing parent directories automatically

---

## 🔐 Set Permissions When Creating a Directory

```bash
mkdir -m 755 new_folder
```

- `-m` sets the permission mode (`755 = rwxr-xr-x`)

---

## ⚠️ Common Errors

- **File exists:** Trying to create a directory that already exists without `-p`
- **Permission denied:** No write permission in the parent directory

---

## 🧪 Useful Options

| Option      | Description                                  |
|-------------|----------------------------------------------|
| `-p`        | Create parent directories as needed          |
| `-v`        | Print a message for each created directory   |
| `-m <mode>` | Set file permissions (e.g., `755`, `700`)    |

---

## 🔁 Examples

### Verbose nested creation
```bash
mkdir -pv project/src/components/utils
```

### Create a directory with restricted access (private)
```bash
mkdir -m 700 secrets
```

---

## ℹ️ More Info

- Manual: `man mkdir`
- Help: `mkdir --help`
- GNU Coreutils: [https://www.gnu.org/software/coreutils/](https://www.gnu.org/software/coreutils/)
