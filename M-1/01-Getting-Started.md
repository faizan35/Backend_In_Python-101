# Getting Started

## Overview of Python

- Python is a high-level, interpreted programming language known for its readability and versatility.
- It is widely used in various domains, including web development, data science, artificial intelligence, and, of course, DevOps.
- Python's simplicity makes it an excellent choice for automating tasks and building scalable systems.

### Understanding the Role of Python in DevOps

- Python plays a crucial role in DevOps by providing a powerful and flexible scripting language.
- It's used for automation, configuration management, and interacting with various tools and APIs in the DevOps toolchain.

### Setting Up Your Python Environment

#### For Windows:

1.  **Install Python:**

    - Visit the [official Python website](https://www.python.org/).
    - Download the latest version of Python for Windows.
    - Run the installer and follow the installation instructions, ensuring you check the box that says "**Add Python to PATH**" during installation.

2.  **Set Up a Virtual Environment:**

    - Open Command Prompt.
    - Navigate to your project folder.
    - Run the following commands:

      ```bash
      python -m venv venv .\venv\Scripts\activate
      ```

    - **Virtual environment** helps keep your project's dependencies isolated, preventing conflicts and easy to manage and share your code.

#### For Linux and macOS:

1.  **Install Python:**

    - Most Linux and macOS distributions come with Python pre-installed. However, you might want to install a newer version using a package manager like `brew` on macOS or `apt` on Debian-based Linux distributions.

    ```bash
    # For macOS using Homebrew
    brew install python

    # For Debian-based Linux
    sudo apt-get update
    sudo apt-get install python3
    ```

2.  **Set Up a Virtual Environment:**

    - Open your terminal.
    - Navigate to your project folder.
    - Run the following commands:

      ```bash
      python3 -m venv venv source venv/bin/activate
      ```

3.  **Verify Your Python Installation:**

    - In the activated virtual environment, run:

      ```bash
      python --version
      ```

      For macOS, you might need to use `python3 --version`.

4.  **Create a "Hello World" Script:**

    - Using a text editor, create a file named `hello.py`.
    - Add the following code:

      ```python
      print("Hello, Python for DevOps!")
      ```

    - Save the file.

5.  **Run the Script:**

    - In your terminal or Command Prompt, navigate to the directory containing `hello.py`.
    - Run the script:

      ```bash
      python hello.py
      ```

      For macOS, you might need to use `python3 hello.py`.

---

## Install a code editor

### 1. **Visual Studio Code (VSCode):**

- Download and install VSCode from the official VSCode website.
- Open VSCode and install Python extension for VSCode from the Extensions view (`Ctrl+Shift+X`).

---
