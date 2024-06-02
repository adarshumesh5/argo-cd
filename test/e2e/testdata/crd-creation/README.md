# Argo CD CRD Creation Example

This example demonstrates how to create an Argo CD application for CRD management.

```
argocd app create crd-creation \
  --repo https://github.com/argoproj/argo-cd.git \
  --path test/e2e/functional/crd-creation \
  --dest-server https://kubernetes.default.svc \
  --dest-namespace default
```

---

## Maintainer

This project is currently maintained by Adarsh Umesh.

-   **Name:** Adarsh Umesh
-   **Title:** Product Manager
-   **Email:** connect2adarshum@gmail.com
-   **LinkedIn:** https://www.linkedin.com/in/adarsh-umesh/

Adarsh is a product management professional with 3+ years of professional experience, skilled in delivering user-focused, scalable solutions.