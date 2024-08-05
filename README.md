
# SonarQube Docker Compose Setup

This repository contains a Docker Compose setup for deploying SonarQube with a MySQL database. It's designed to help developers quickly set up SonarQube for code quality analysis, particularly for .NET Core projects. 

## Overview

SonarQube is an open-source platform that helps you manage code quality by providing continuous code inspection and analysis for bugs, vulnerabilities, and code smells. This setup leverages Docker Compose to simplify the deployment process.

## Prerequisites

Before you begin, ensure you have the following installed on your system:

- **Docker**: [Install Docker](https://www.docker.com/products/docker-desktop)
- **Docker Compose**: [Install Docker Compose](https://docs.docker.com/compose/install/)
- **Java JDK 11 or 17**: [Install Java](https://www.oracle.com/java/technologies/javase-downloads.html) (SonarQube requires Java to run)

## Setup Instructions

### Step 1: Clone the Repository

Clone this repository to your local machine:

```bash
git clone https://github.com/b3r3ch1t/sonarqube.git
cd sonarqube
```

### Step 2: Configure the Docker Compose File

The repository includes a `docker-compose.yml` file that sets up both SonarQube and a MySQL database. The setup includes custom container names and a restart policy to ensure stability.

### Step 3: Start the Containers

Run the following command to start the SonarQube and MySQL containers:

```bash
docker-compose up -d
```

This command will download the necessary Docker images (if not already available) and start the containers in the background.

### Step 4: Access SonarQube

After starting the containers, you can access SonarQube by navigating to:

```
http://localhost:9000
```

The default login credentials are:

- **Username:** `admin`
- **Password:** `admin`

You will be prompted to change the password upon your first login.

## Integrating with .NET Core Projects

To integrate SonarQube with your .NET Core projects, follow the steps outlined in [this article](https://medium.com/@anderson.meneses/mastering-code-quality-with-sonarqube-a-step-by-step-guide-to-integration-with-docker-compose-and-597146433133) which provides a detailed guide.

## Integrating with DevOps and CI/CD Tools

Integrating SonarQube with your CI/CD pipeline is highly recommended to ensure continuous monitoring of code quality. Tools like Jenkins, Azure DevOps, and GitHub Actions can be easily configured to include SonarQube in your build process.

## Read the Full Article on Medium

For a detailed guide on setting up and integrating SonarQube with Docker Compose and .NET Core, check out the full article on Medium:

[Mastering Code Quality with SonarQube: A Step-by-Step Guide](https://medium.com/@anderson.meneses/mastering-code-quality-with-sonarqube-a-step-by-step-guide-to-integration-with-docker-compose-and-597146433133)

## Connect with Me

Let's connect on LinkedIn:

[Anderson Meneses on LinkedIn](https://www.linkedin.com/in/anderson-meneses)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributions

Contributions are welcome! Please submit a pull request or open an issue to suggest improvements or report bugs.

## Contact

For any questions or support, feel free to contact the repository owner via [GitHub](https://github.com/b3r3ch1t).
