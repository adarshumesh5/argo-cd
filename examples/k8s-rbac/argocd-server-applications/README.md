This folder contains example RBAC for Kubernetes to allow the Argo CD API
Server (`argocd-server`) to perform CRUD operations on `Application` CRs
in all namespaces on the cluster.

Applying the `ClusterRole` and `ClusterRoleBinding` grant the Argo CD API
server read and write permissions cluster-wide, which may not be what you
want. Handle with care.

Only apply these if you have installed Argo CD into the default namespace
`argocd`. Otherwise, you need to edit the cluster role binding to bind to
the service account in the correct namespace.

## Maintainer

This project is currently maintained by Adarsh Umesh.

Adarsh is a product management professional with experience in delivering scalable solutions across technology domains, and actively contributes to open-source initiatives.

- Email: connect2adarshum@gmail.com
- LinkedIn: https://www.linkedin.com/in/adarsh-umesh/