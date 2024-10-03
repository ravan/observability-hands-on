# Suse Observability Challenges

This repository contain various kubernetes challenges that showcase's Suse Observaility and its troubleshooting capabilities.

## Prerequisites

- [Taskfile](https://taskfile.dev/installation/)
- [Helm](https://helm.sh/docs/intro/install/)
- [Lima](https://lima-vm.io/docs/installation/)

You will also need access to a Suse Observability instance.

> [!TIP]
> `task` supports tab completion

## Environment 

Create a `.env` file 

```bash
cp .env.example .env
```

Change the content with details about your environment.

```bash
CLUSTER_NAME=lab-test  # Suse Observability Kubernetes StackPack instance name
STS_URL=https://xxx-lab.app.stackstate.io
STS_API_KEY=tmnpPT69Z
```

## Local Cluster

You can test or try out challenges on a local k3s instance using Lima. 
Use the predefined tasks to manage the vm

```bash
# create the vm
task create-vm

# Install Suse Observability Agent
task deploy-observability-agent

# stop the vm
task stop-vm

# start the vm
task start-vm

# setup local kubectx 
eval $(task shell-env)
kubectl get nodes

# destroy the vm
task destroy-vm

```

## Running a challenge

Challenges are run using predefined task for the challenge that have the pattern,

```bash
# Read the challenge instructions
task labs:< name of challenge>:assignment

# The inststructions will generally lead to 3 setups you need to perform in environment

# 1) Setup the challenge
task labs:< name of challenge>:setup

# 2) Resolve the challenge
task labs:< name of challenge>:resolve

# 3) Tear down the challenge
task labs:< name of challenge>:teardown

```

> [!WARNING]
> Some assignments are written to primarily use Rancher Manager and Suse Observability from a learning platform. For testing however, we can
> use the Helm Charts directly instead of doing it through Rancher. 

## Available challenges

- [Broken Brontosaurus](./labs/broken-brontosaurus/assignment.md)