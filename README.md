
# Daily Task Automation Script

## Overview
This Python script automates the organization of files in a specified folder by their creation date. It simplifies file management by sorting files into subfolders named by date.

## Features
- Automatically creates subfolders based on the creation date of files.
- Moves files into respective date-named subfolders.
- User-friendly and easy to execute.

## Requirements
- Python 3.6 or higher.
- Operating system with file system access.

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/bian4all/daily-task-automation.git
   ```
2. Navigate to the project folder:
   ```bash
   cd daily-task-automation
   ```

## Usage
1. Open a terminal and run the script:
   ```bash
   python organize_files.py
   ```
2. Enter the folder path you want to organize when prompted.

## Example
If you have the following folder structure:
```
MyFolder
├── file1.txt
├── file2.jpg
├── file3.docx
```
After running the script, it will look like this:
```
MyFolder
├── 2024-12-12
│   ├── file1.txt
│   ├── file2.jpg
├── 2024-12-11
│   ├── file3.docx
```

## Contributing
Contributions are welcome! Please fork the repository, make changes, and submit a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
Created by **bian4all**
