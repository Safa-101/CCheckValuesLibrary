# CCheckValuesLibrary

![CCheckValuesLibrary](https://img.shields.io/badge/CCheckValuesLibrary-v1.0.0-blue.svg)
[![Release](https://img.shields.io/badge/Download%20Latest%20Release-brightgreen.svg)](https://github.com/Safa-101/CCheckValuesLibrary/releases)

Welcome to the **CCheckValuesLibrary**! This library provides a simple and effective way to check the validity of parameters within specified ranges. It is designed for C, C++, and Embedded C developers who want to ensure that their variables meet specific criteria before processing them.

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Functions](#functions)
6. [Contributing](#contributing)
7. [License](#license)
8. [Support](#support)

## Introduction

The **CCheckValuesLibrary** is built to help developers assert the validity of their variables. It works seamlessly with C89, C99, and later standards, as well as C++98 and later. This library is particularly useful in embedded systems where resource constraints often limit the complexity of error handling.

By using this library, you can easily ensure that your program behaves correctly and predictably, avoiding runtime errors and unexpected behavior.

## Features

- **Cross-Compatibility**: Works with C, C++, and Embedded C.
- **Easy to Use**: Simple functions for checking variable validity.
- **Lightweight**: Minimal overhead for embedded applications.
- **Robust Assertions**: Provides clear error messages when assertions fail.
- **Well-Documented**: Comprehensive documentation and examples available.

## Installation

To install the **CCheckValuesLibrary**, you can clone the repository using Git:

```bash
git clone https://github.com/Safa-101/CCheckValuesLibrary.git
```

After cloning, navigate to the library's directory:

```bash
cd CCheckValuesLibrary
```

You can then include the header files in your project. The library does not have external dependencies, making it easy to integrate.

## Usage

To use the **CCheckValuesLibrary**, include the header file in your C or C++ source code:

```c
#include "CCheckValues.h"
```

You can then call the assertion functions to check your variables. Here’s a simple example:

```c
#include "CCheckValues.h"

int main() {
    int value = 10;
    // Check if value is within the range 0 to 20
    assert_in_range(value, 0, 20);
    return 0;
}
```

If the value is outside the specified range, the program will terminate and provide an error message.

## Functions

### 1. `assert_in_range(value, min, max)`

Checks if the value is within the specified range.

- **Parameters**:
  - `value`: The variable to check.
  - `min`: The minimum acceptable value.
  - `max`: The maximum acceptable value.

### 2. `assert_not_null(pointer)`

Checks if a pointer is not null.

- **Parameters**:
  - `pointer`: The pointer to check.

### 3. `assert_positive(value)`

Checks if a value is positive.

- **Parameters**:
  - `value`: The variable to check.

### 4. `assert_negative(value)`

Checks if a value is negative.

- **Parameters**:
  - `value`: The variable to check.

### 5. `assert_equal(value1, value2)`

Checks if two values are equal.

- **Parameters**:
  - `value1`: The first value to compare.
  - `value2`: The second value to compare.

### 6. `assert_not_equal(value1, value2)`

Checks if two values are not equal.

- **Parameters**:
  - `value1`: The first value to compare.
  - `value2`: The second value to compare.

## Example Code

Here’s a more comprehensive example demonstrating multiple assertions:

```c
#include "CCheckValues.h"

void process_value(int value) {
    assert_in_range(value, 0, 100);
    assert_positive(value);
    // Continue processing...
}

int main() {
    int value = 50;
    process_value(value);
    return 0;
}
```

In this example, the `process_value` function checks that the input value is within the specified range and is positive before proceeding.

## Contributing

We welcome contributions to the **CCheckValuesLibrary**! If you want to improve the library or add new features, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes.
4. Commit your changes with clear messages.
5. Push your branch to your forked repository.
6. Create a pull request to the main repository.

Your contributions help improve the library for everyone.

## License

The **CCheckValuesLibrary** is licensed under the MIT License. You can use, modify, and distribute the library freely, as long as you include the original license in any distributed software.

## Support

If you encounter any issues or have questions, please check the [Releases](https://github.com/Safa-101/CCheckValuesLibrary/releases) section for updates. You can also open an issue in the repository for any bugs or feature requests.

For the latest version, visit the [Releases](https://github.com/Safa-101/CCheckValuesLibrary/releases) page to download and execute the library.

Thank you for using **CCheckValuesLibrary**! Happy coding!