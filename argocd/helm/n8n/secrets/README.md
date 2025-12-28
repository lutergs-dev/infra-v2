### Secrets in n8n-postgresql

maintain secret values needs to use in n8n postgresql DB.

copy-paste `secrets-raw-example.yaml` to `secrets-raw.yaml`, and fill out data by given instruction.

!! please remind do not post original `secrets-raw.yaml` to git.

and create sealed-secret via execute this command.

```shell
kubeseal --controller-name=sealed-secrets --controller-namespace=sealed-secrets -o yaml < secrets-raw.yaml > secrets.yaml
```


### Secrets in n8n-encryption-key

maintain secret values needs to use in n8n master - worker encryption key.

copy-paste `encryption-key-raw-example.yaml` to `encryption-key-raw.yaml`, and fill out data by given instruction.

!! please remind do not post original `encryption-key-raw.yaml` to git.

and create sealed-secret via execute this command.

```shell
kubeseal --controller-name=sealed-secrets --controller-namespace=sealed-secrets -o yaml < encryption-key-raw.yaml > encryption-key.yaml
```

