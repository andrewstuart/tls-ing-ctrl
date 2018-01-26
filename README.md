# tls-ing-ctrl

An attempt to create an ideal abstraction layer for obtaining Kubernetes Ingress
TLS Certificates atop modern PKI automation solutions, such as [Let's
Encrypt](/letsencrypt) and [Vault](/hashicorp/vault).

## Design

- Ingress Controller sets tls-ing-ctrl as the default secure backend.
  - This allows SNI requests to pass through automatically to the backend.
