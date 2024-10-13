- Here’s a summary of the file navigation and essential Git commands, along with example code for each:
- To move to the root directory in Git Bash, you can use the following command:

### Move to Root Directory

- **Command**: `cd /`
- **Description**: Changes the current directory to the root of the file system.

### Example

```bash
cd /
```

or

```bash
cd ~
```

After executing this command, you will be in the root directory of your file system.

- If you are on Windows, this will take you to the root of the current drive (like `C:`),
- while on Unix-like systems (Linux, macOS, git bash), it will take you to the root of the entire file system.

### File Navigation Commands in Git Bash

1.  **Moving Upward**:

    - **Command**: `cd ..` or `cd ../` or `cd ../..`
    - **Description**: Moves up one directory level (to the parent directory).
    - **Example**:

      ```bash
      cd ..

      cd ../

      cd ../..
      ```

2.  **Moving Downward**:

    - **Command**: `cd [directory_name]`
    - **Description**: Moves into a specified subdirectory.
    - **Example**:

      ```bash
      cd documents

      skyde@SEL MINGW64 ~
      $ cd /d/Dcode/devNotes/sass
      skyde@SEL MINGW64 /d/Dcode/devNotes/sass

      skyde@SEL MINGW64 ~
      $ cd /d/Dcode/devNotes/sass
      skyde@SEL MINGW64 /d/Dcode/devNotes/sass
      ```

````

3. **Combining Levels**:
   - **Upward multiple levels**:
     - **Command**: `cd ../..`
     - **Example**:
       ```bash
       cd ../..
       ```
   - **Downward multiple levels**:
     - **Command**: `cd folder1/folder2`
     - **Example**:
       ```bash
       cd folder1/folder2
       ```
