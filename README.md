# k8s-guide

## Prerequisites

### aws-cli
Install:
[https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)

Configure:
`aws configure`

Set profile:
`export AWS_PROFILE=<profile>`

### kubectl
Install:
[https://kubernetes.io/docs/tasks/tools/](https://kubernetes.io/docs/tasks/tools/)

### Install eksctl
Install:
[https://eksctl.io/installation/](https://eksctl.io/installation/)

Create cluster:
`eks create cluster --name <cluster-name> --region <region-code>`


## Context
`aws eks update-kubeconfig --name <cluster-name> --region <region-code>`
`# kubectl config delete-context <context-name>`
`# kubectl config unset clusters.<cluster-name>`
`# kubectl config unset users.<username>`

## Kubectl cheatsheet
[https://kubernetes.io/docs/reference/kubectl/quick-reference/](https://kubernetes.io/docs/reference/kubectl/quick-reference/)

### Create namespace
`kubectl create ns <namespace>`

### Use namespace
`kubectl -n <namespace>`

### Port-Forward
`kubectl port-forward <pod-name> <local-port>:<pod-port>`

### Logs
`kubectl logs <pod-name> -f`