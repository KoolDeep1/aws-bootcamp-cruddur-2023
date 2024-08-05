# Week 0 — Billing and Architecture

## Required Homework

### Install and verify AWS CLI

I installed the AWS CLI on Gitpod via iTerm. I followed the instructions for the Linux installation from the [AWS CLI Install Documentation Page](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)

See the updtated Gitpod.Yaml file under AWS folder. Attaching the code below for convenience:

```
tasks:
  - name: aws-cli
    env:
      AWS_CLI_AUTO_PROMPT: on-partial
    init: |
      cd /workspace
      curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
      unzip awscliv2.zip
      sudo ./aws/install
      cd $THEIA_WORKSPACE_ROOT
vscode:
  extensions:
    - 42Crunch.vscode-openapi
```

You can see in the screenshot bellow that the installation was successful:

![installing AWS CLI](assets/proof_of_aws_cli.png)

## Homework Challenges

