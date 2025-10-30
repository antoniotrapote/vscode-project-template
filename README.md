# VSCode Project Template
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC_BY--NC--SA_4.0-black?logo=creativecommons&logoColor=white)](LICENSE)

A minimal and clean template for Python projects in Visual Studio Code.  
It includes a preconfigured `.vscode` folder for environment auto-activation and Copilot instruction files.

---

## Prerequisites

Before you start, make sure you have:
- **Python 3.10 or higher** installed on your system. Check by running: `python --version`
- **Visual Studio Code** installed. [Download here](https://code.visualstudio.com)
- **Basic terminal knowledge** - you'll be running commands in the terminal

If you don't have Python installed, visit [python.org](https://www.python.org/downloads/) to download and install it first.

---

## How to use this template

1. Click the green "Use this template" button at the top of this page to create a new repository based on this template.
2. Clone your new repository to your local machine.
3. Open the project folder in Visual Studio Code.

## Setup

### 1. Create and activate a virtual environment

Open a **new integrated terminal** in VS Code:
- Press `` Cmd+` ``
- Or use the menu: *Terminal → New Terminal*

A virtual environment is an isolated Python setup for your project. It prevents conflicts between different projects' dependencies.

Run these commands in the terminal:

```bash
# Create a new virtual environment (Python 3.12 recommended)
python -m venv .venv

# Activate it (macOS / Linux)
source .venv/bin/activate

# On Windows (PowerShell)
.venv\Scripts\Activate.ps1
```

**Success indicator**: Your terminal prompt should now show `(.venv)` at the beginning, like `(.venv) user@computer project %`

---

### 2. Verify that everything works

Run this command in the **same terminal** to confirm that Python is using the correct virtual environment:

```bash
python -c "import sys, os; print('Python:', sys.executable); print('VIRTUAL_ENV:', os.environ.get('VIRTUAL_ENV'))"
```

Expected output:

```
Python: /path/to/your/project/.venv/bin/python
VIRTUAL_ENV: /path/to/your/project/.venv
```

If both paths match your project folder, your environment is set up correctly ✅

---

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

**What is this?** The `requirements.txt` file lists all Python packages your project needs. This template starts empty, so you can add packages as needed. For example:

```
requests==2.31.0
pytest==7.4.0
```

To add a new package, install it with `pip install package_name` and then update `requirements.txt`.

---

### 4. Run your scripts

Create a Python file in your project folder, for example `main.py`:

```python
print("Hello from my first Python project!")
```

Then run it in the terminal:

```bash
python main.py
```

VS Code will automatically detect and use the `.venv` environment you created earlier. ✅

---

## 📁 Structure

```
.github/               # Copilot and coding standards instructions
.vscode/               # VS Code settings (auto-enables your virtual environment)
.gitignore             # Tells Git to ignore .venv and temporary files
.venv/                 # Your virtual environment (created when you run python -m venv .venv)
AGENTS.md              # Documentation about AI assistant usage in this workspace
LICENSE                # Project license (CC BY-NC-SA 4.0)
README.md              # This file
requirements.txt       # Python package dependencies for your project
```

---

## 🚀 Next Steps

1. **Start coding** - Create Python files in your project folder
2. **Add dependencies** - Install packages with `pip install package_name`
3. **Write tests** - Create test files following the project's Python coding standards
4. **Use Copilot** - Follow the coding standards in `.github/` for AI-assisted development

For detailed coding standards, see [`.github/instructions/python.instructions.md`](.github/instructions/python.instructions.md)

---

## 🐛 Troubleshooting

### Virtual environment not activated?
- **macOS/Linux**: Make sure you ran `source .venv/bin/activate` in the terminal
- **Windows**: Make sure you ran `.venv\Scripts\Activate.ps1`
- Check that your prompt shows `(.venv)` at the beginning

### `python: command not found`?
- Python might not be installed or not in your PATH
- Run `python --version` or `python3 --version` to check
- If using `python3`, replace `python` with `python3` in all commands

### VS Code doesn't recognize the virtual environment?
- Reload VS Code: `Cmd+Shift+P` → "Developer: Reload Window"
- Or restart VS Code completely
- The `.vscode` settings should auto-detect your `.venv` folder

### Still stuck?
- Check that you're in the correct project folder
- Make sure all steps in the Setup section were completed in order
- Try opening a new terminal in VS Code

---

## ⚖️ License

CC BY-NC-SA 4.0 &copy; 2025 [Antonio L. Martínez Trapote](https://github.com/antoniotrapote) 
