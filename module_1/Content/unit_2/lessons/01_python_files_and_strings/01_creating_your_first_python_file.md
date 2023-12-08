So far, we've been writing fairly simple Python code in the interactive shell. While the interactive shell remains to be a good option to quickly run and evaluate Python code, it's not suitable for larger and more complex programs. In order to have more flexibility in what we're building, we'll need to write our own custom Python files.

## What is a Python File?

It's a text file where you can write Python code. It ends with the `.py` extension. These code files are essentially text files that can be written using any text editor, like Notepad on Windows or TextEdit on Mac. However, in order to write code faster and in a more organized fashion, we'll need to use a code editor.

## What is a Code Editor?

Code editors are text editors that are designed to help programmers write code effectively and efficiently. Most code editors come with helper tools and features that assist programmers write more code in less time. Some of these features include —— but are not limited to:

- Code auto completion (in certain contexts)
- Code highlighting (for better visibility)
- Code formatting (for better readability)

Visual Studio Code (VS Code) is currently the most popular code editor in the market. It's free, open source and is available for all major operating systems (Windows, Mac, Linux).

## Installing Visual Studio Code

Head to the [downloads](https://code.visualstudio.com/download) section on VS code website and select the appropriate version for your operating system.

Follow the on-screen instructions to finalize the installation process.

## Creating Your First Python File

Proceed with the following steps:
- On your desktop, create a folder called `code`.
- Open Visual Studio Code and open the folder you just created.

![opening folders in vscode](//images.ctfassets.net/nbtht4kjx2t0/6zRNC0WU8xstU0XYIXLOvv/a8abc3f2554ffa39ed0ace5b231890c4/opening_folders_in_vscode.png)
- Click on the "New File" icon to add a new file. Name it `script.py`
![creating new file vscode](//images.ctfassets.net/nbtht4kjx2t0/1qjfMQ4NHBF2d47rxmRZmT/035b0eacddc2f63c49fc17aae8e4e85e/creating_new_file_vscode.png)

> The names `code` and `script.py` are not requirements to write Python files. You can give any names to your folders and Python files. Just make sure your Python files end with the `.py` extension.

## Running a Python File

To see how Python files are executed, let's write some code.

In your `script.py` file, add the following code:

```python
user_name = "Alan Turing"
occupation = "Computer Scientist"
print(user_name + " was a brilliant " + occupation)
```

To run the file, open VS code built-in terminal.
![open new terminal vscode](//images.ctfassets.net/nbtht4kjx2t0/2yomc0cMU1rDf6MKGQFApg/e7940759d5d840ea7cfea0c588344c95/open_new_terminal_vscode.png)

Type the command `python` followed by the file name.

```shell
python script.py
```

> If you are on Mac and you are using the Python version installed from the official website, you need to use the command `python3` instead.

![executing file in terminal vscode](//images.ctfassets.net/nbtht4kjx2t0/62bBWr6UkNXxA5Yb1QLhAa/51e6fea09ba0e49259043cc083dc61b1/executing_file_in_terminal_vscode.png)

> Don't worry if your terminal looks different from the one in the screenshot. It's just a different theme.

Voila! The program ran successfully and the message was printed in the terminal.

In the next concept, we'll dive deeper into more string operations.



