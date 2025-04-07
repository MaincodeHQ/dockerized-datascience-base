# Dockerized Data Science Base

A ready-to-use development container for data science projects with pre-configured tools and libraries.

## Quick Start

### Prerequisites

- [Docker](https://www.docker.com/products/docker-desktop/) installed on your system
- [VS Code](https://code.visualstudio.com/) with the [Dev Containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

### Using the Dev Container

1. Clone the repository:
   ```bash
   git clone https://github.com/MaincodeHQ/dockerized-datascience-base.git
   cd dockerized-datascience-base
   ```

2. Open the project in VS Code:
   ```bash
   code .
   ```

3. When prompted, click "Reopen in Container" or use the command palette (F1) and select "Dev Containers: Reopen in Container"

4. VS Code will build and start the dev container automatically. This may take a few minutes the first time.

5. Once inside the dev container, start the environment:
   ```bash
   task up
   ```
   This command will build and start all required services defined in the docker-compose file.

### Sharing Your Project

When you need to share your project with collaborators:

1. From within the dev container, run:
   ```bash
   task zip
   ```

2. This will generate a zip file of the entire project that's ready to be emailed or uploaded.

3. Recipients can then:
   - Extract the zip file
   - Open the folder in VS Code with the Dev Containers extension
   - Run `task up` to recreate the exact same environment

## Features

- Ready-to-use data science environment with Python, Jupyter, and common libraries
- Pre-configured VS Code dev container setup
- Task automation for common operations
- Easy sharing with collaborators


## License

This project is licensed under the MIT License - see the LICENSE file for details.

---

Maintained by [MaincodeHQ](https://github.com/MaincodeHQ)