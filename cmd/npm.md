Here's a list of commonly used npm commands, including the ones you mentioned:

### 1. Initialize a New Project
- **`npm init`**: Initializes a new Node.js project and creates a `package.json` file.
- **`npm init -y`**: Initializes a new project with default settings (no prompts).

### 2. Show Installed Packages
- **Local Packages**: 
  - **`npm list`**: Shows all installed packages in the current project.
  - **`npm list --depth=0`**: Shows only top-level packages (without their dependencies).
  
- **Global Packages**:
  - **`npm list -g --depth=0`**: Lists globally installed packages.

### 3. Install Packages
- **Install a Dependency**:
  - **`npm install <package-name>`**: Installs a package and adds it to the `dependencies` section in `package.json`.
  
- **Install a Development Dependency**:
  - **`npm install <package-name> --save-dev`**: Installs a package and adds it to the `devDependencies` section.
  
- **Install All Dependencies**:
  - **`npm install`**: Installs all dependencies listed in `package.json`.

- **Install a Global Package**:
  - **`npm install -g <package-name>`**: Installs a package globally.

### 4. Uninstall Packages
- **Uninstall a Dependency**:
  - **`npm uninstall <package-name>`**: Uninstalls a package and removes it from `package.json`.

- **Uninstall a Global Package**:
  - **`npm uninstall -g <package-name>`**: Uninstalls a global package.

### 5. Additional Useful Commands
- **Update Packages**:
  - **`npm update <package-name>`**: Updates a specific package.
  
- **Check for Outdated Packages**:
  - **`npm outdated`**: Lists outdated packages in the current project.

- **Run a Script**:
  - **`npm run <script-name>`**: Runs a script defined in `package.json`.

This should cover the main npm commands you might need for managing packages in your Node.js projects!