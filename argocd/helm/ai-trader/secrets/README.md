

```shell
kubeseal --controller-name=sealed-secrets --controller-namespace=sealed-secrets -o yaml < docker-credential-raw.yaml > docker-credential.yaml
```


```shell
kubeseal --controller-name=sealed-secrets --controller-namespace=sealed-secrets -o yaml < generic-credential-raw.yaml > generic-credential.yaml
```

