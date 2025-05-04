# Using the Python Interpreter

## Invoking the Interpreter
- Typically installed as `/usr/local/bin/python3.11`
- Run via `python3.11` (Unix) or `py` / `python3.11` (Windows)
- End interpreter with:
  - `Ctrl+D` (Unix) or `Ctrl+Z` (Windows)
  - `quit()` function
- Supports line editing (if Readline available):
  - Try `Ctrl+P` to test
- Runs:
  - Interactively (via terminal)
  - Scripts: `python script.py`
  - Commands: `python -c 'command'`
  - Modules: `python -m module`
  - Interactive mode after script: `python -i script.py`

## Argument Passing
- Arguments stored in `sys.argv` (from `import sys`)
- `sys.argv[0]` varies:
  - Script name / `-` / `-c` / module name
- Arguments after `-c` or `-m` passed to command/module

## Interactive Mode
- Prompted with `>>>` (primary) and `...` (secondary)
- Shows version info on start
- Example:
  ```python
  the_world_is_flat = True
  if the_world_is_flat:
      print("Be careful not to fall off!")

