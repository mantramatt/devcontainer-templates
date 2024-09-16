# DevContainer Templates

This project contains development container templates for various environments. These templates are designed to streamline the setup process for development environments and ensure consistency across different projects. The templates will be updated periodically to incorporate new features and improvements.

## Table of Contents

- [DevContainer Templates](#devcontainer-templates)
  - [Table of Contents](#table-of-contents)
  - [Introduction to DevContainers](#introduction-to-devcontainers)
  - [React](#react)
    - [React Development Container](#react-development-container)
    - [React VS Code Extensions](#react-vs-code-extensions)
  - [CosmWasm](#cosmwasm)
    - [CosmWasm Development Container](#cosmwasm-development-container)
    - [CosmWasm VS Code Extensions](#cosmwasm-vs-code-extensions)
  - [Go + Ignite](#go--ignite)
    - [Go + Ignite Development Container](#go--ignite-development-container)
    - [Go + Ignite VS Code Extensions](#go--ignite-vs-code-extensions)
  - [Getting Started](#getting-started)
    - [React](#react-1)
    - [CosmWasm](#cosmwasm-1)
    - [Go + Ignite](#go--ignite-1)
  - [Contributing](#contributing)
  - [License](#license)

## Introduction to DevContainers

[DevContainers](https://code.visualstudio.com/docs/remote/containers) are a feature of Visual Studio Code that allow you to open any folder inside (or mounted into) a container and take advantage of Visual Studio Code's full feature set. DevContainers are defined by a `.devcontainer` folder in the root of your project, which contains a `devcontainer.json` file that specifies the container configuration.

To use a DevContainer, include the `.devcontainer` folder in the root of your project and open the project in Visual Studio Code. You will be prompted to reopen the project in the container.

## React

The React development container is based on the `mcr.microsoft.com/devcontainers/typescript-node:1-20-bullseye` image. This container is pre-configured with essential tools and extensions to facilitate React development.

### React Development Container

The development container for React includes the following configurations:

- **Base Image**: `mcr.microsoft.com/devcontainers/typescript-node:1-20-bullseye`
- **VS Code Settings**: Customizable settings for a tailored development experience.
- **VS Code Extensions**: Pre-installed extensions to enhance productivity.

### React VS Code Extensions

The following VS Code extensions are included in the React development container:

- `esbenp.prettier-vscode`: Code formatter for consistent styling.
- `dbaeumer.vscode-eslint`: Linter for identifying and fixing code issues.

## CosmWasm

The CosmWasm development container is based on the `mcr.microsoft.com/devcontainers/rust:1-1-bullseye` image. This container is tailored for developing CosmWasm smart contracts using Rust.

### CosmWasm Development Container

The development container for CosmWasm includes the following configurations:

- **Base Image**: `mcr.microsoft.com/devcontainers/rust:1-1-bullseye`
- **VS Code Settings**: Customizable settings for a tailored development experience.
- **VS Code Extensions**: Pre-installed extensions to enhance productivity.
- **Post Create Command**: Automatically installs the `cosmwasm-check` tool after the container is created.

### CosmWasm VS Code Extensions

The following VS Code extensions are included in the CosmWasm development container:

- `rust-lang.rust-analyzer`: Provides Rust language support.
- `vadimcn.vscode-lldb`: Debugger for Rust.
- `dtsvet.vscode-wasm`: WebAssembly support for VS Code.

## Go + Ignite

The Go + Ignite development container is based on the `mcr.microsoft.com/devcontainers/go:1.16` image. This container is configured for developing applications using Go and the Ignite framework.

### Go + Ignite Development Container

The development container for Go + Ignite includes the following configurations:

- **Base Image**: `mcr.microsoft.com/devcontainers/go:1.16`
- **VS Code Settings**: Customizable settings for a tailored development experience.
- **VS Code Extensions**: Pre-installed extensions to enhance productivity.

### Go + Ignite VS Code Extensions

The following VS Code extensions are included in the Go + Ignite development container:

- `golang.go`: Provides Go language support.
- `ms-vscode.go`: Additional Go tools for VS Code.
- `ignite-cli.ignite`: Ignite CLI support for VS Code.

## Getting Started

To get started with any of the projects, open the respective directory in Visual Studio Code and reopen it in the container when prompted.

### React

1. Open the `react/` directory in Visual Studio Code.
2. Reopen in the container when prompted.
3. Run `yarn install` to install dependencies.

### CosmWasm

1. Open the `cosmwasm/` directory in Visual Studio Code.
2. Reopen in the container when prompted.
3. The `cosmwasm-check` tool will be installed automatically.

### Go + Ignite

1. Open the `go-ignite/` directory in Visual Studio Code.
2. Reopen in the container when prompted.
3. Run `go mod tidy` to install dependencies.

## Contributing

Please follow the guidelines for each project when contributing.

## License

This project is licensed under the MIT License.