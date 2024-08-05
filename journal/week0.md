# Week 0 — Billing and Architecture

## Required Homework

### Install and verify AWS CLI

I installed the AWS CLI on Gitpod via iTerm. I followed the instructions for the Linux installation from the [AWS CLI Install Documentation Page](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html).

Here's the installation command:
```
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
```

See the updtated Gitpod.Yaml file under AWS folder. Attaching the code below for convenience:

```
# Gitpod configuration file for setting up the development environment

tasks:
  - name: aws-cli  # Task name for AWS CLI installation
    env:
      AWS_CLI_AUTO_PROMPT: on-partial  # Enables auto-prompt for AWS CLI
    init: |
      # Navigate to the workspace directory
      cd /workspace
      
      # Download the AWS CLI installation package for Linux
      curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
      
      # Unzip the downloaded package
      unzip awscliv2.zip
      
      # Run the installation script
      sudo ./aws/install
      
      # Navigate back to the workspace root
      cd $THEIA_WORKSPACE_ROOT

# List of VS Code extensions to be installed in the development environment
vscode:
  extensions:
    - 42Crunch.vscode-openapi  # Extension for OpenAPI (Swagger) support```

You can see in the screenshot bellow that the installation was successful:

![installing AWS CLI](assets/proof_of_aws_cli.png)

## Homework Challenges

