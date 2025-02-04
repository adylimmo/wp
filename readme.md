# Add SSL from file

```
kubectl create secret tls my-tls-secret --cert=ca_bundle.crt --cert=certificate.crt --key=private.key
```