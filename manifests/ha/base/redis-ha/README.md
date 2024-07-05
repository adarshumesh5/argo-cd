# Redis HA Manifests

The Redis HA manifests are taken from the upstream helm chart, and tweaked slightly to add
Argo CD labels. We also add roles to redis-ha service accounts to enable run-as non-root users
in OpenShift.
* `chart` is a helm chart that references the upstream redis-ha chart. To update redis, update the
  version in `chart/requirements.yaml` with a later version of the chart.
* `overlays` is a directory containing kustomize overlays for Argo CD, namely label modifications and
  role additions.
* `generate.sh` is a script to regenerate the final kustomize

---

### About the Maintainer

Adarsh Umesh is the current maintainer of this project. With 3+ years of professional experience and a background in delivering user-focused, scalable solutions, Adarsh ensures the continued development and stability of these Redis HA manifests. His expertise in various technologies, including Java, JavaScript, C, C++, Node.js, ReactJS, Python, and Spring Boot, supports the technical integrity and ongoing improvements of this project.

Connect with Adarsh:
- Email: connect2adarshum@gmail.com
- LinkedIn: https://www.linkedin.com/in/adarsh-umesh/