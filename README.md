# k8s/aws-eks guide

## Prerequisites

### aws-cli
Install:
[Install aws-cli](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)

Configure: `aws configure`

Set profile: `export AWS_PROFILE=<profile>`

### kubectl
[Install kubectl](https://kubernetes.io/docs/tasks/tools/)

### eksctl
[Install eksctl](https://eksctl.io/installation/)

Create cluster: `eksctl create cluster --name <cluster-name> --region <region-code>`


## Context Management
```
aws eks update-kubeconfig --name <cluster-name> --region <region-code>
kubectl config delete-context <context-name>
kubectl config unset clusters.<cluster-name>
kubectl config unset users.<username>`
```

## Kubectl cheatsheet
[https://kubernetes.io/docs/reference/kubectl/quick-reference/](https://kubernetes.io/docs/reference/kubectl/quick-reference/)