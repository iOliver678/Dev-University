# Beginner Guide: What is a Python VM and How to Create One

## What is a Python VM?

A Python VM (virtual environment) is an isolated environment where you can run Python code and install packages without affecting your system Python or other projects. It keeps dependencies clean and project-specific.

## Why Use It?

- Keeps project dependencies separate
- Prevents conflicts between packages
- Avoids needing admin permissions
- Easy to replicate environments with `requirements.txt`

## How to Create a Python Virtual Environment

### 1. Create a project folder

```
mkdir my_project
cd my_project
```

### 2. Create the virtual environment

```
python3 -m venv venv
```

This creates a folder named `venv/` containing the isolated Python environment.

### 3. Activate the environment

**On macOS/Linux:**

```
source venv/bin/activate
```

**On Windows:**

```
venv\Scripts\activate
```

When active, your terminal prompt will change to show `(venv)`.

### 4. Install packages

```
pip install requests
```

### 5. Save installed packages (optional)

```
pip freeze > requirements.txt
```

### 6. Deactivate the environment

```
deactivate
```

## Quick Reference

| Command                         | Description                     |
| ------------------------------- | ------------------------------- |
| `python3 -m venv venv`          | Create virtual environment      |
| `source venv/bin/activate`      | Activate (macOS/Linux)          |
| `venv\Scripts\activate`         | Activate (Windows)              |
| `deactivate`                    | Exit the environment            |
| `pip install <package>`         | Install a package               |
| `pip freeze > requirements.txt` | Save installed packages to file |
