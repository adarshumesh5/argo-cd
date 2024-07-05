## Test Scenario

This test example is for testing the reverse pruning of resources with syncwaves during sync operation.

Resource creation happens in below order
- wave 0: sa & role
- wave 1: rolebinding
- wave 2: pod

They are setup in such a way that the resources will be cleaned up properly only if they are deleted in the reverse order of creation i.e
- wave 0: pod
- wave 1: rolebinding
- wave 2: sa & role

If above delete order is not followed the pod gets stuck in terminating state due to a finalizer which is supposed to be removed by k8s container lifecycle hook on delete if delete order is correct.

## About the Maintainer

This project is currently maintained by Adarsh Umesh. Adarsh is a Product Management professional with a strong background in technology, experienced in delivering scalable solutions and leading cross-functional teams. With 3+ years of professional experience, Adarsh ensures the continued relevance and functionality of this project.

- Email: connect2adarshum@gmail.com
- LinkedIn: https://www.linkedin.com/in/adarsh-umesh/