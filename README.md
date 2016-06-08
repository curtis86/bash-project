# bash-project

## A. Summary

Quickly generate a simple BASH project from a set of template files. Apart from setting up the project structure, some of the following functions are provided in bash-project:

 * Text formatting (bold, normal, green, red and yellow)
 * Trap control
 * Message and error printing
 * File/directory access check
 * Yes/No prompt
 * Script usage function
 * String to uppwer/lower
 * Dependency checker

Feel free to use as your own/improve on.

## B. Dependencies

BASH 4 or later (may require some adjustments to work with older versions of BASH).

## C. Supported Systems

Any nix or BSD system with BASH 4 or later (may require some adjustments to work with older versions of BASH).

### Installation

1. Clone this repo to your preferred directory (eg: /opt/bash-project)

  `git clone https://github.com/curtis86/bash-project`

### Usage

  ```
  ./bash-project <project_name> <project_parent_directory>
  ```

Included functions can be found in the `includes/bp.sh` file in your created project. Note that functions included by bash-project are prefixed with `bp`, ie: `bp::msg`

### Usage example

  ```
  ./bash-project my_new_project /Users/curtis/Code

  Are you sure you want to create project my_new_project 0.1 in /Users/curtis/Code (/Users/curtis/Code/my_new_project/) ? <y/n> y

  Creating project...

  Completed. Project created in /Users/curtis/Code/my_new_project.
  ```

This will create a project called "my_new_project" in directory /Users/curtis/Code/my_new_project .

### Projects that use bash-project

 * [solar-flare-alert](https://github.com/curtis86/solar-flare-alert)
 * [tinc-mgr](https://github.com/curtis86/tinc-mgr)

### Reserved names

```
abrt
check_dependencies
force_exit
home_dir
HOME_DIR
INCLUDES_DIR
main
PROJECT_NAME
SCRIPT_DEPENDENCIES
t_bold
t_green
t_normal
t_red
t_yellow
test_access
usage
```

### Notes

1. Please ensure that the project_parent_directory already exists (eg: /home/user/code).
2. Please do not use 'special' characters in project names.

## License

The MIT License (MIT)

Copyright (c) 2016 Curtis K

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
