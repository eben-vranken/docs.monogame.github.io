---
title: Setting up your development environment for VSCode
description: A step-by-step guide for setting up your development IDE using VSCode
---

This is a guide on setting up your development IDE for creating games with MonoGame using Visual Studio Code. By following this guide, you will learn how to install the necessary tools for developing C# applications and configure Visual Studio Code with recommended extensions for C# development.

By the end, you will be fully equipped to start creating games with MonoGame using Visual Studio Code.

## Install Visual Studio Code

### [Windows](#tab/windows)

1. Open your web browser and navigate to [https://code.visualstudio.com/](https://code.visualstudio.com/).

    ![Download VSCode](./images/1_setting_up_your_development_environment/vscode/windows/download-vscode.png)

2. Click the **Download for Windows** button.  This will redirect you to the download page where the installer will automatically download.
3. When the download completes, run the installer and complete the steps to install Visual Studio Code.

### [macOS](#tab/macos)

1. Open your web browser and navigate to [https://code.visualstudio.com/](https://code.visualstudio.com/).

    ![Download VSCode](./images/1_setting_up_your_development_environment/vscode/mac/download-vscode.png)

2. Click the **Download Mac Universal** button.  This will redirect you to the page where the application archive (.zip) file will begin downloading.
3. Extract the contents of the VSCode archive that downloaded by double-clicking it inside a Finder window.  This will extract the **Visual Studio Code.app** file.
4. Drag the **Visual Studio Code.app** file into the **Applications** folder, making it available in the macOS Launchpad.

### [Ubuntu](#tab/ubuntu)

1. Open your web browser and navigate to [https://code.visualstudio.com/](https://code.visualstudio.com/).

    ![Download VSCode](./images/1_setting_up_your_development_environment/vscode/linux/download-vscode.png)

2. Click the Download `.deb` button.
3. Double click the `.deb` file and press the `Install` button.

---

## Setting up VS Code for development with MonoGame

1. Open Visual Studio Code
1. Open up its terminal window (`Ctrl/Cmd` + `J`)
1. Run the following command to install MonoGame Templates

    ```sh
    dotnet new install MonoGame.Templates.CSharp
    ```

## Install Visual Studio Code C# Extensions

To transform Visual Studio Code from a simple text editor into a powerful development environment for C# projects, you must install the Visual Studio Code C# extension. This extension enhances the editor by providing syntax highlighting, code analysis, IntelliSense, and other features that significantly improve the development experience and productivity when working with C#.

1. Open Visual Studio Code.
2. Click the **Extensions** icon in the **Activity Bar** on the left.

    ![Click Extensions](./images/1_setting_up_your_development_environment/vscode/click-extensions.png)

3. In the **Search Box** type `C#`.
4. Click **Install** for the **C# Dev Kit** extension.  Installing this will also install the base **C#** extension.

![Install C# DevKit Extension](./images/1_setting_up_your_development_environment/vscode/install-devkit.png)

## (Optional) Install the "MonoGame for VSCode" extension

A community member has built a VSCode extension for VS code to enable:

- Automatically install MonoGame templates
- Create new projects from the file menu or command palette
- Open the MGCB editor with the click of a button (very useful)

You can find this extension by following the steps above and searching for "MonoGame for VS Code" by r88.

> [!NOTE]
> While not built by the MonoGame team, we regularly use this extension ourselves and fully support it.

## Creating a new MonoGame project

1. Open up an empty folder in Visual Studio Code
1. Open up its terminal window (`Ctrl/Cmd` + `J`)
1. Run the following command to create an empty project for desktop platforms:

    ```sh
    dotnet new mgdesktopgl
    ```

1. When VS Code asks you about automatic creation of launch / task files, press yes
1. You can now press F5 to compile and debug you game, happy coding  :)

## Next Steps

Next, get to know MonoGame's code structure and project layout:

- [Understanding the code](3_understanding_the_code.md)