
# Advanced Python Terminal

> A feature-rich cross-platform command-line terminal with file management, system utilities, image processing, and data analysis capabilities.

&#x20;

## Table of Contents

* [Features](#features)
* [Installation](#installation)
* [Usage](#usage)
* [Command Reference](#command-reference)

  * [File Operations](#file-operations)
  * [Text Processing](#text-processing)
  * [Image Processing](#image-processing)
  * [Data Analysis](#data-analysis)
  * [System Utilities](#system-utilities)
  * [Math Utilities](#math-utilities)
  * [Other Commands](#other-commands)
* [Contributing](#contributing)
* [License](#license)

## Features

* **File Operations**: Manage files and directories (create, read, write, delete, copy, rename)
* **Text Processing**: Search, count, and pretty-print text, JSON, and YAML
* **Image Processing**: Cartoonify, sketch, and comic book effects
* **Data Analysis**: View CSV files and generate simple plots
* **System Utilities**: Networking tools (ping, DNS lookup, speed test), weather lookup, timezones, system info
* **Math Utilities**: Calculations, conversions, greatest common divisor, least common multiple
* **Help & Navigation**: Built-in `help`, `clr`, `dt`, and directory utilities

## Installation

1. Ensure you have **Python 3.8+** installed:

   ```bash
   python --version
   ```
2. Install dependencies via pip:

   ```bash
   pip install opencv-python numpy pandas matplotlib pyyaml pytz scikit-image speedtest-cli googletrans==4.0.0-rc1
   ```
3. Clone or download this repository.

## Usage

Follow these steps to get started and explore all features:

1. **Launch the Terminal**
   Open your shell/terminal and run:

   ```bash
   python terminal.py
   ```

   You will see a prompt like `>>>`, indicating the app is ready.

2. **Access the Help Menu**
   At any time, type:

   ```bash
   help
   ```

   This lists every command with a brief description. Handy for navigation.

3. **Navigate Directories**

   * List files and folders:

     ```bash
     cdir
     ```
   * Change into a folder:

     ```bash
     cd projects
     ```
   * Return to the home directory:

     ```bash
     cd ~
     ```

4. **Manage Files**

   * Read a file:

     ```bash
     read notes.txt
     ```
   * Create or overwrite a file (interactive):

     ```bash
     write diary.txt
     ```
   * Append text to an existing file:

     ```bash
     append log.txt
     ```
   * Remove a file:

     ```bash
     remove temp.txt
     ```

5. **Text & Data Inspection**

   * Search for text inside files:

     ```bash
     find report.md "TODO"
     ```
   * Pretty-print JSON or YAML:

     ```bash
     json config.json
     yaml settings.yaml
     ```
   * View first 10 lines of a CSV:

     ```bash
     f data.csv 10
     ```

6. **Perform Calculations**

   * Simple math:

     ```bash
     calc "(5+3)*2"
     ```
   * Temperature conversion:

     ```bash
     tconv 1 100   # 100°C to Kelvin
     ```

7. **Network & System Tools**

   * Check internet speed:

     ```bash
     speedtest
     ```
   * Ping a host:

     ```bash
     ping example.com
     ```
   * Look up DNS records:

     ```bash
     dns-lookup example.com
     ```

8. **Image Processing**

   * Convert images to cartoon style:

     ```bash
     cartoonify photo.jpg cartoon.png
     ```
   * Create a pencil sketch:

     ```bash
     sketch portrait.png sketch.png
     ```

9. **Exiting & Clearing**

   * Clear the screen buffer:

     ```bash
     clr
     ```
   * Quit the terminal interface:

     ```bash
     exit
     ```

10. **Shortcuts & Tips**

    * Use the **Up/Down arrow keys** to cycle through command history.
    * Tab completion is supported for file and directory names.
    * You can chain OS shell commands by prefixing with `shell`, e.g.:

      ```bash
      shell ls -la
      ```

Once you’re comfortable, explore other specialized commands (image, translation, bill splitting, weather lookup, etc.) via the `help` menu. Enjoy your advanced Python terminal!

## Command Reference

### File Operations

| Command         | Description                 | Example           |
| --------------- | --------------------------- | ----------------- |
| `cdir`          | List directory contents     | `cdir`            |
| `cd <dir>`      | Change directory            | `cd documents`    |
| `read <file>`   | Display file contents       | `read notes.txt`  |
| `write <file>`  | Create/edit file via prompt | `write diary.txt` |
| `append <file>` | Append to file via prompt   | `append log.txt`  |
| `remove <file>` | Delete file                 | `remove temp.txt` |
| `mkdir <dir>`   | Create directory            | `mkdir projects`  |
| `rmdir <dir>`   | Remove empty directory      | `rmdir old_files` |
| `tree [dir]`    | Show directory tree         | `tree src/`       |
| `stat <file>`   | Show file statistics        | `stat image.jpg`  |

### Text Processing

| Command                 | Description                      | Example                |                  |
| ----------------------- | -------------------------------- | ---------------------- | ---------------- |
| `find <file> <text>`    | Search for text in file          | `find log.txt "error"` |                  |
| `grep <pattern> <file>` | Regular expression search        | \`grep "warning        | error" log.txt\` |
| `json <file>`           | Pretty-print JSON                | `json config.json`     |                  |
| `yaml <file>`           | Pretty-print YAML                | `yaml settings.yaml`   |                  |
| `languages`             | List supported translation codes | `languages`            |                  |

### Image Processing

| Command                       | Description              | Example                     |
| ----------------------------- | ------------------------ | --------------------------- |
| `cartoonify <image> [output]` | Convert to cartoon       | `cartoonify photo.jpg`      |
| `sketch <image> [output]`     | Convert to pencil sketch | `sketch portrait.png`       |
| `comic <image> [output]`      | Apply comic book effect  | `comic picture.jpg art.png` |

### Data Analysis

| Command                        | Description                | Example                  |
| ------------------------------ | -------------------------- | ------------------------ |
| `f <csv> [n]`                  | Show first n rows of a CSV | `f data.csv 20`          |
| `plot <csv> <column> [output]` | Plot a CSV column          | `plot sales.csv revenue` |

### System Utilities

| Command              | Description                | Example                  |
| -------------------- | -------------------------- | ------------------------ |
| `ping <host>`        | Ping network host          | `ping google.com`        |
| `traceroute <host>`  | Trace network route        | `traceroute example.com` |
| `dns-lookup <host>`  | DNS lookup                 | `dns-lookup example.com` |
| `weather <location>` | Show weather summary       | `weather New York`       |
| `speedtest`          | Internet speed test        | `speedtest`              |
| `sysinfo`            | Display system information | `sysinfo`                |
| `timezones`          | List all IANA timezones    | `timezones`              |

### Math Utilities

| Command                             | Description                      | Example              |
| ----------------------------------- | -------------------------------- | -------------------- |
| `calc <expr>`                       | Evaluate mathematical expression | `calc "5*(3+2)"`     |
| `gcd <a> <b>`                       | Greatest common divisor          | `gcd 48 18`          |
| `lcm <a> <b>`                       | Least common multiple            | `lcm 6 8`            |
| `tconv <type> <val>`                | Temperature conversions (C↔F↔K)  | `tconv 1 100`        |
| `splitbill <total> <people> [tip%]` | Split a bill among people        | `splitbill 100 4 15` |

### Other Commands

| Command       | Description                        |
| ------------- | ---------------------------------- |
| `help`        | Show all commands and descriptions |
| `clr`         | Clear the terminal screen          |
| `dt`          | Display current date and time      |
| `pwd`         | Print working directory            |
| `shell <cmd>` | Execute a shell command            |

## Contributing

Contributions are welcome! Please fork the repository, create a new branch, and submit a pull request. Ensure your code follows PEP 8 and includes tests for new features.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
