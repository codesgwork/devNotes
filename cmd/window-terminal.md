To display a list of files and folders in a directory using the Windows Command Prompt, you can use the `dir` command. Here’s how to do it:

### Command to List Files and Folders

1. **Basic Command**:
   ```bash
   dir
   ```

In the context of the Windows file system, the "root" directory usually refers to the top-level directory of a specific drive. Here’s a breakdown:

- **Root of C: Drive**: When you refer to the root of the C: drive, it means `C:\`, which is the highest level of the C: drive.

```bash
cd \
```

### Example Commands:

```bash
   D:\Dcode\CSSLearn>c:

   C:\Users\skyde>D:

   D:\Dcode\CSSLearn>cd /

   D:\>c:

   C:\Users\skyde>cd /

   C:\>c:

   C:\>cd \Users\skyde

   C:\Users\skyde>
```

Here are some basic Windows Command Prompt (CMD) commands for navigating files and directories, creating files and folders, and moving around the directory structure:

- **Clear the Command Prompt screen**:
  ```bash
  cls
  ```

### Navigating Directories

1. **Open a specific folder**:

   ```bash
   cd path\to\your\folder
   ```

   Example:

   ```bash
   cd C:\Users\YourUsername\Documents
   ```

2. **Go up one directory**:

   ```bash
   cd ..
   ```

3. **Go back to the previous directory**:

   ```bash
   cd -
   ```

4. **List all files and folders in the current directory**:

   ```bash
   dir
   ```

5. **Change to the root directory of the current drive**:
   ```bash
   cd \
   ```

### Creating Files and Folders

1. **Create a new folder**:

   ```bash
   mkdir FolderName
   ```

   Example:

   ```bash
   mkdir MyNewFolder
   ```

2. **Create a new text file**:

   ```bash
   echo. > filename.txt
   ```

   Example:

   ```bash
   echo. > myfile.txt
   ```

3. **Create multiple folders at once**:
   ```bash
   mkdir Folder1 Folder2 Folder3
   ```

### Moving Files and Folders

1. **Move a file from one directory to another**:

   ```bash
   move path\to\source\file.txt path\to\destination\
   ```

   Example:

   ```bash
   move C:\Users\YourUsername\Documents\file.txt C:\Users\YourUsername\Desktop\
   ```

2. **Rename a file or folder**:
   ```bash
   ren OldName NewName
   ```
   Example:
   ```bash
   ren oldfile.txt newfile.txt
   ```

### Deleting Files and Folders

1. **Delete a file**:

   ```bash
   del filename.txt
   ```

   Example:

   ```bash
   del myfile.txt
   ```

2. **Delete a folder and its contents**:
   ```bash
   rmdir /s /q FolderName
   ```
   Example:
   ```bash
   rmdir /s /q MyNewFolder
   ```
