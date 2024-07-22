# Testing certificates

This directory contains all TLS certificates used for testing ArgoCD, including
the E2E tests. It also contains the CA certificate and key used for signing the
certificates.

* `argocd-test-ca.crt` and `argocd-test-ca.key` are the CA
* `argocd-test-client.crt` and `argocd-test-client.key` is a client certificate/key pair, signed by the CA
* `argocd-test-server.crt` and `argocd-test-server.key` is a server certificate/key pair, signed by the CA, with its CN set to 'localhost', and SAN entry for IP 127.0.0.1.

All keys have no passphrase. All certs, including CA cert, are valid until July
2119, so there should be no worries about having to renew them.

You can use the CA certificate to sign more certificates, if you need additional
certificates for testing.

Needless to say, but should be mentioned anyway: Do not use these certs for 
anything else except Argo CD tests.

---

## About the Maintainer

This project is currently maintained by Adarsh Umesh.

Adarsh is a Product Management professional with 5+ years of experience, skilled in delivering user-focused, scalable solutions across finance and technology domains. He actively maintains projects, aligning technical feasibility with strategic goals.

**Contact:**
*   Email: connect2adarshum@gmail.com
*   LinkedIn: https://www.linkedin.com/in/adarsh-umesh/