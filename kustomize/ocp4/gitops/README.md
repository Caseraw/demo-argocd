# Installing OpenShift GitOps (ArgoCD)

This is an example setup for ArgoCD using the OpenShift GitOps Operator. It uses
and enhances the existing Cluster ArgoCD instance that comes with the Operator.

## Platforms

It's tried and tested on:
- OpenShift 4.10

## Requirements

- Properly functioning OCP 4.10 cluster.
- A proper user and Permissions to install the Operator.
- `oc` cli to apply the initial Kustomize setup.

## Installation

Clone the repository:

`git clone https://github.com/Caseraw/demo-argocd.git`

Apply the resources:

`oc apply -k github_repo/kustomize/ocp4/gitops`

## Resources

- https://github.com/argoproj-labs/argocd-operator
- https://github.com/argoproj-labs/argocd-operator/tree/master/examples
- https://argocd-operator.readthedocs.io/en/latest/install/openshift
- https://argo-cd.readthedocs.io/en/stable
- https://developers.redhat.com/learn/openshift/develop-gitops
- https://developers.redhat.com/courses/gitops/getting-started-argocd-and-openshift-gitops-operator
- https://cloud.redhat.com/blog/introduction-to-gitops-with-openshift
- https://demo.openshift.com/en/latest/argocd
