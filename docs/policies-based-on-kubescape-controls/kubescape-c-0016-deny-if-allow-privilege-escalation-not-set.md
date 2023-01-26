# Kubescape C-0016: Deny if allowPrivilegeEscalation is not set

## Why this policy is required:
Attackers may gain access to a container and uplift its privilege to enable excessive capabilities.

## Severity Level: Medium

## Configuration Parameters:
* Not Configurable

## Resources this policy could be applied to:
* CronJob
* DaemonSet
* Deployment
* Job
* Pod
* ReplicaSet
* StatefulSet

## What does this policy do:
### This Policy checks for every container in the resource:
* If `resources.limits.memory` `resources.limits.cpu`

## Implementing this policy in the Cluster:
[Refer here for using the policy in the cluster](https://github.com/kubescape/cel-admission-library#using-the-library)