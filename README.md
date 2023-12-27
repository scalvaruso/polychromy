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

Polychromy is a Python script to manipulate the colors of a text.

## Features

- Function ```colorate``` prints text of a specified colour in a specified colour background.
- Function ```show``` prints out color details such as Hex and RGB values of a given colour in a square of the given colour.

## Latest Version 1.0.1

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
  from polychromy import colorate
```

## Usage

Calling the function ```colorate``` inside your program will return a printable string of the desired color.

### Parameters

The function accept most color names, RGB values ```[0-255];[0-255];[0-255]```, Hex values ```#[00-FF][00-FF][00-FF]```, xterm color number in the format ```x[0-255]```, and ANSI codes.[^Note]

[^Note]: The output color might differ from the desired one depending on terminal used.

### Examples

Here are some examples of how to use polychromy.

<!--- Example 01 --->
#### Show

Using the function ```show``` you can print out color details such as Hex and RGB values of a given colour in a square of the given colour.

```Python
import sys
from polychromy import show

# If you run this program without any argument it asks you for a color and prints it out to the screen.
if len(sys.argv) == 1:

    color_in = input("Enter a colour: ")
    show(color_in)

# Giving a color as argument it prints it out directly to the screen
# Accepted values are: Name colors, HEX and RGB values.

else:
    show()

```

##### Output 1

![example01](https://raw.githubusercontent.com/scalvaruso/polychromy/main/images/example01.png)

<!--- Example 02 --->
#### Colorate

Using the function ```colorate``` you can print text of a specified colour in a specified colour background.

```Python
from polychromy import colorate

# Texts to print
text1 = "There are only 10 kinds of people in this world:"
text2 = "Those who know binary and Those who don't."

# Foreground (text) coors
foreground_1 = "#F5F5F5"
foreground_2 = 90

# Background colors
background_1 = "0;128;128"
background_2 = "Cosmic Latte"

print(colorate(text1,foreground_1,background_1))
print(colorate(text2,foreground_2,background_2))

```

##### Output 2

![example02](https://raw.githubusercontent.com/scalvaruso/polychromy/main/images/example02.png)

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
