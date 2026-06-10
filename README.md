# Automating Python Projects with Pip, PyPi & Scripting

## Overview

This project is a Python automation tool developed as part of the **Module Lab: Automating Python Projects with Pip, PyPi & Scripting**.

The application generates timestamped log files from user-provided log entries and demonstrates the use of:

* Python scripting
* File I/O operations
* Dependency management with pip
* Automated testing with pytest
* Reproducible environments using `requirements.txt`

## Features

* Creates log files with timestamped filenames.
* Writes log entries to a text file.
* Validates user input before processing.
* Raises exceptions for invalid input.
* Supports execution from the command line.
* Includes automated tests using pytest.

## Project Structure

```text
.
├── lib/
│   └── generate_log.py
├── testing/
│   └── test_generate_log.py
├── requirements.txt
├── README.md
└── pytest.ini
```

## Installation

### Clone the Repository

```bash
git clone <your-forked-repository-url>
cd course-7-module-6-pip-pypi-scripting-lab
```

### Create a Virtual Environment (Optional)

```bash
python -m venv venv
```

Activate the environment:

**Linux/macOS**

```bash
source venv/bin/activate
```

**Windows**

```bash
venv\Scripts\activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

## Usage

Run the Python script:

```bash
python generate_log.py
```

Example output:

```text
Log written to log_20260610.txt
```

A log file will be created in the project directory containing the provided log entries.

## Example Function

```python
from lib.generate_log import generate_log

log_data = [
    "User logged in",
    "User updated profile",
    "Report exported"
]

generate_log(log_data)
```

## Running Tests

Execute the test suite with:

```bash
pytest -v
```

Expected result:

```text
5 passed
```

## Dependencies

Dependencies are tracked in:

```text
requirements.txt
```

Generate or update the file with:

```bash
pip freeze > requirements.txt
```

## Skills Demonstrated

* Python File I/O
* Functions and input validation
* Exception handling
* Dependency management with pip
* Reproducible development environments
* Automated testing with pytest
* Git and GitHub workflow

## Author

Vincent

