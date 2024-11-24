Please try to write a standalone python file `reproducer.py` to reproduce the issue. Put the file in a code block.

The file would be put in the root directory of the project and executed by `python3 reproducer.py`. The script should raise an `AssertionError` when the issue is present and print a stack trace of the issue. The script should also exit with code 0 when the issue is fixed.

Please use the following function to print the stack trace, so that the line numbers of the statements are shown clearly:
```
def print_stacktrace(e: Exception):
    import traceback
    import sys
    tb = traceback.extract_tb(e.__traceback__)
    print("Traceback (most recent call last):", file=sys.stderr)
    for frame in tb:
        line_number = frame.lineno
        code_context = frame.line.strip() if frame.line else "Unknown"
        print(f'  File \"{frame.filename}\"', file=sys.stderr)
        print(f"    {line_number}: {code_context}", file=sys.stderr)
    print(f"{e.__class__.__name__}: {e}", file=sys.stderr)
```
