# Polychromy

[<img src="https://img.shields.io/badge/polychromy-py-blue?style=flat&logo=python&logoWidth=20.svg/"></a>](https://github.com/scalvaruso/polychromy/)
[![PyPI - Version](https://img.shields.io/pypi/v/polychromy?logo=pypi&logoColor=white&color=blue)](https://pypi.org/project/polychromy/)
[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/polychromy?logo=python)](https://pypi.org/project/polychromy/)
[![Downloads](https://static.pepy.tech/badge/polychromy)](https://pepy.tech/project/polychromy)
[![PyPI - License](https://img.shields.io/pypi/l/polychromy?color=blue)](https://github.com/scalvaruso/polychromy/blob/main/LICENSE.md)

<!---
[![PyPI - status](https://img.shields.io/pypi/status/:polychromy)](https://pypi.org/project/polychromy/)
[![Documentation Status](https://readthedocs.org/projects/polychromy/badge/?version=latest)](https://polychromy.readthedocs.io/en/latest/?badge=latest)
-->

## Description

Polychromy is a Python script to manipulate the color of text.

## Features

- Prints text of a specified colour in a specified colour background.
- Prints out Hex and RGB values of a given colour in a square of the given colour.

## Latest Version 0.0.2

## Table of Contents

- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
  - [Parameters](#parameters)
  - [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)

## Getting Started

### Prerequisites

This script relies on the Python standard library and ```textlinebreaker```.

### Installation

- Install the package with pip

```bash
  pip install polychromy
```

- Import the package in your program

```Python
  from polychromy import color_show
```

## Usage

Calling the function ```color_show()``` inside your program will print a square of the color given as input to the function, and its HEX and RGB values.

### Parameters

... _to be completed_ ...

### Examples

```Python
import sys
from polychromy import color_show

# If you run this program without any argument it asks you for a color and prints it out to the screen.
if len(sys.argv) == 1:

    color_in = input("Enter a colour: ")
    color_show(color_in)

# Giving a color as argument it prints it out directly to the screen
# Accepted values are: Name colors, HEX and RGB values.

else:
    color_show()

```

## Contributing

If you'd like to contribute to this project, please follow these steps:

1. Fork the repository on GitHub.
2. Clone the fork to your local machine.
3. Create a new branch for your feature or bug fix.
4. Make your changes and commit them.
5. Push the changes to your fork on GitHub.
6. Create a pull request to the original repository.

## License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/scalvaruso/polychromy/blob/main/LICENSE.md) file for details.
