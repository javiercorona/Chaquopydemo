# Advanced Python Terminal

> A feature-rich cross-platform command-line terminal with file management, system utilities, image processing, and data analysis capabilities.

[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)](https://www.python.org/) [![License: MIT](https://img.shields.io/badge/license-MIT-green)](#license)

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

Run the terminal interface:

```bash
python terminal.py
```

Type `help` to see the full list of available commands.

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
