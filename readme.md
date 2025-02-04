# Add SSL from file from zero ssl

```
cat dev.anakdevops.online/certificate.crt dev.anakdevops.online/ca_bundle.crt > dev.anakdevops.online/gabung.crt
kubectl create secret tls my-tls-secret --cert=dev.anakdevops.online/gabung.crt --key=dev.anakdevops.online/private.key


kubectl create secret tls my-tls-secret --cert=dev.anakdevops.online/gabung.crt --key=dev.anakdevops.online/private.key --dry-run=client -o yaml > dev-wp-nginx/templates/secret-ssl.yaml

```