# K8s-beginner-to-advanced
Repository to store and contribute the K8s journey from Beginner to Advanced

- Creating deployments and services

- Using namespaces in your deployments and services

- Using Ingress Controller and resources
    - Some useful commands -
    - `minikube addons enable ingress`
    - `openssl genpkey -algorithm RSA -out tls.key -pkeyopt rsa_keygen_bits:2048`
    - `openssl req -new -key tls.key -out tls.csr`
    - `openssl x509 -req -in tls.csr -signkey tls.key -out tls.crt -days 365`
    - Generate a private key
        - `openssl genpkey -algorithm RSA -out tls.key -pkeyopt rsa_keygen_bits:2048`
    - Generate a CSR
        - `openssl req -new -key tls.key -out tls.csr`
    - Generate a self-signed certificate
        - `openssl x509 -req -in tls.csr -signkey tls.key -out tls.crt -days 365`
    - Create a Kubernetes secret
        - `kubectl create secret tls example-tls --cert=tls.crt --key=tls.key`
    
    


- What is Helm package manager?

- Using Volumes and understanding persistent volume claims

- What is a StatefulSet?

