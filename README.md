# Runner Template Repository

This repository serves as a template for running various scripts with different services, such as Git, Docker, and [UV](https://docs.astral.sh/uv/). Currently, it supports UV with Git and Alembic, with plans to expand support for additional services, including Docker, in the future.

> **Note:** It's a new repo, so if you find any bugs, please let me know via issues

## Script Overview

The script provided automates the installation, configuration, and management of a service. It includes functions for:

- **Checking dependencies**: Verifies the required system and Python packages are installed.
- **Cloning the repository**: Fetches the script source code from GitHub.
- **Managing the service**: Supports starting, stopping, restarting, and checking the status of the service.
- **Logging**: Captures both standard and error logs during execution.
- **Uninstalling the service**: Completely removes the installation, service files, and logs.


### Notes:
- **Installation**: This script installs the necessary dependencies and prepares the service for running.
- **Service Management**: Start, stop, or restart the service with systemd commands.
- **Logging**: Logs are written to a specified log file for easy tracking of service operations.


## Installation

1. **Fork this repository** to your own account.
2. **Customize the installation script** according to your needs.

## Usage

After completing the installation, you can use the following commands:

- **Install Script**:

  - public repo:
    ```bash
    sudo bash -c "$(curl -sL {GITHUB_INSTALL_URL})" @ install-script
    ```

  - private repo:
    ```bash
    sudo bash -c "$(curl -H 'Authorization: token {GITHUB_TOKEN}' -sL {GITHUB_INSTALL_URL})" @ install-script
    ```

- **Install the source**:
  ```bash
  {SCRIPT_NAME} install
  ```

- **Install the service**:
  ```bash
  {SCRIPT_NAME} install-service
  ```

- **Start the service and run the source**:
  ```bash
  {SCRIPT_NAME} start
  ```

- **Stop the service**:
  ```bash
  {SCRIPT_NAME} stop
  ```

- **Restart the service**:
  ```bash
  {SCRIPT_NAME} restart
  ```

- **View status**:
  ```bash
  {SCRIPT_NAME} status
  ```

- **View logs**:
  ```bash
  {SCRIPT_NAME} logs
  ```

- **Update the script**:
  ```bash
  {SCRIPT_NAME} update
  ```

- **Uninstall the service**:
  ```bash
  {SCRIPT_NAME} uninstall
  ```


## Contact & Support

- Telegram Channel: [@ErfJabs](https://t.me/ErfJabs)

Feel free to ⭐ the project to show your support!

[![Stargazers over time](https://starchart.cc/erfjab/runner.svg?variant=adaptive)](https://starchart.cc/erfjab/runner)