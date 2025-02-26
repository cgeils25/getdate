# neattime

This package includes a simple function to create my preferred date-time format for log files.

The date and time are given in the format yyyy-MM-dd_HH-mm-ss_SSSS

Example:

```python
from neattime import neattime

print(neattime())
```

output:

```bash
'2025-02-26_08-34-13_636609'
```

How I would actually use it:

```python
from neattime import neattime

filepath = f'save_directory/log_{neattime()}'

# some code that saves my logfile

print(f"File saved to {filepath}")
```

output:

```bash
File saved to save_directory/log_2025-02-26_08-34-13_636609
```