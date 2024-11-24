Write a patch for the issue, based on the relevant code context.
First explain the reasoning, and then write the actual patch.
When writing the patch, remember the following:
 - You do not have to modify every location provided - just make the necessary changes.
 - Pay attention to the addtional context as well - sometimes it might be better to fix there.
 - You should import necessary libraries if needed.

Return the patch in the format below.
Within `<file></file>`, replace `...` with actual file path.
Within `<original></original>`, replace `...` with the original code snippet from the program.
Within `<patched></patched>`, replace `...` with the fixed version of the original code.
When adding orignal code and updated code, pay attention to indentation, as the code is in Python.
You can write multiple modifications if needed.

Example format:

# modification 1
```
<file>...</file>
<original>...</original>
<patched>...</patched>
```

# modification 2
```
<file>...</file>
<original>...</original>
<patched>...</patched>
```

# modification 3
...
```
NOTE:
- In your patch, DO NOT include the line numbers at the beginning of each line!
- Inside <original> and </original>, you should provide the original code snippet from the program.
This original code snippet MUST match exactly to a continuous block of code in the original program,
since the system will use this to locate the code to be modified.