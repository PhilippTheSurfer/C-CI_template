# C Program Compilation with GitHub Actions

This repository demonstrates the power and flexibility of GitHub Actions for automating C program compilation. It provides a basic setup for compiling C code, showcasing how GitHub Actions can be leveraged for continuous integration and development workflows in C projects.

## Purpose

The main goal of this repository is to serve as an educational tool for understanding and implementing GitHub Actions in C programming projects. It includes a simple C program as a starting point and a GitHub Actions workflow that compiles the program upon every push to the repository.

## Getting Started

To get started with this repository, you can fork it to your account or clone it directly to your local machine using:


### Prerequisites

- A GitHub account
- Basic knowledge of git commands
- GCC compiler installed locally (for testing the C program locally)

## How the Action Works

The GitHub Action workflow is defined in `.github/workflows/compile.yml`. It triggers on every `push` event to the repository. The workflow performs the following steps:

1. Checks out the code from the repository to the GitHub Actions runner.
2. Installs GCC on the runner.
3. Compiles the C program using GCC.
4. Optionally, runs the compiled program.

## Adding Your C Program

To add your own C program to the repository:

1. Place your C source files in the root directory or a specific directory of your choice.
2. If you placed your C files in a different directory, modify the `compile.yml` workflow file to change the working directory or specify the path to your C file in the compile command.
3. Commit and push your changes to GitHub.

## Workflow Customization

You can customize the workflow by editing the `.github/workflows/compile.yml` file. For example, you can add more build steps, integrate with other tools or services, or configure the workflow to run on different events or branches.

## Contributing

Contributions to this project are welcome. Please feel free to fork the repository, make your changes, and submit a pull request.

