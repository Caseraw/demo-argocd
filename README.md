# Example setup for OpenShift GitOps (ArgoCD)

An example setup that utilizes the OpenShift GitOps Operator to setup an ArgoCD demo instance. Use it for setting up labs, testing and or learning purposes.

## Platforms

It's tried and tested on:
- OpenShift 4.10

## Requirements

- Properly functioning OCP 4.10 cluster.
- A proper user and Permissions to install the Operator.
- `oc` cli to apply the initial Kustomize setup.

# Usage

## Installation

Clone the repository:

`git clone https://github.com/Caseraw/demo-argocd.git`

> If needed, make your own changes to the contents.

Install the OpenShift GitOps Operator:

`oc apply -k kustomize/openshift-gitops/install`

Install the *demo-instance-argocd* ArgoCD Instance:

`oc apply -k kustomize/demo-instance-argocd`

## Uninstall

Docs:
- https://docs.openshift.com/container-platform/4.10/cicd/gitops/uninstalling-openshift-gitops.html

# Resources

- https://docs.openshift.com/container-platform/4.10/cicd/gitops/gitops-release-notes.html
- https://github.com/argoproj-labs/argocd-operator
- https://github.com/argoproj-labs/argocd-operator/tree/master/examples
- https://argocd-operator.readthedocs.io/en/latest/install/openshift
- https://argo-cd.readthedocs.io/en/stable
- https://github.com/redhat-developer/openshift-gitops-getting-started
- https://developers.redhat.com/learn/openshift/develop-gitops
- https://developers.redhat.com/courses/gitops/getting-started-argocd-and-openshift-gitops-operator
- https://cloud.redhat.com/blog/introduction-to-gitops-with-openshift
- https://demo.openshift.com/en/latest/argocd
