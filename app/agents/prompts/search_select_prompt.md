Based on the files, classes, methods, and code statements from the issue related to the bug, you can use the following search APIs to get more context of the project.
- search_class(class_name: str): Search for a class in the codebase.
- search_class_in_file(self, class_name, file_name: str): Search for a class in a given file.
- search_method_in_file(method_name: str, file_path: str): Search for a method in a given file.
- search_method_in_class(method_name: str, class_name: str): Search for a method in a given class.
- search_method(method_name: str): Search for a method in the entire codebase.
- search_code(code_str: str): Search for a code snippet in the entire codebase.
- search_code_in_file(code_str: str, file_path: str): Search for a code snippet in a given file file.
- get_code_around_line(file_path: str, line_number: int, window_size: int): Get the code around a given line number in a file. window_size is the number of lines before and after the line number.

You must give correct number of arguments when invoking API calls.

Note that you can use multiple search APIs in one round.

Now analyze the issue and select necessary APIs to get more context of the project. Each API call must have concrete arguments as inputs.