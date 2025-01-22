# SonarQube Setup and Configuration Ansible Role

This Ansible role automates the installation and configuration of SonarQube, PostgreSQL, and Nginx for reverse proxy setup on a target machine. It includes setting up SonarQube with a PostgreSQL backend and configuring Nginx as a reverse proxy for SonarQube.

## Prerequisites

- Ansible installed on your local machine.
- A target machine running a supported version of Ubuntu/Debian.
- Sudo or root access on the target machine.
- Ensure the target machine has at least 2GB of RAM and sufficient disk space.
- OpenJDK 17 or higher is required for running SonarQube.

## Role Variables

This role doesn't have any configurable variables by default. You can modify the configuration by changing the appropriate properties directly in the tasks.

## Dependencies

- None

## Installation

You can install this role via Ansible Galaxy or manually. Here's how to use it:

### Option 1: Clone the repository

Clone the repository to your Ansible project's `roles` directory:

```bash
git clone https://example.com/your-ansible-role.git /path/to/your/ansible/project/roles/sonarqube
