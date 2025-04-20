### Secrets in ghost-mysql

maintain secret values needs to use in ghost MySQL DB.

copy-paste `secrets-raw-example.yaml` to `secrets-raw.yaml`, and fill out data by given instruction.

!! please remind do not post original `secrets-raw.yaml` to git.

and create sealed-secret via execute this command.

```shell
kubeseal --controller-name=sealed-secrets --controller-namespace=sealed-secrets -o yaml < secrets-raw.yaml > secrets.yaml
```


### Secrets in ghost-smtp-setting

maintain secret values needs to use in ghost Amazon SES mail setting.

copy-paste `mail-secrets-raw-example.yaml` to `mail-secrets-raw.yaml`, and fill out data by given instruction.

!! please remind do not post original `mail-secrets-raw.yaml` to git.

and create sealed-secret via execute this command.

```shell
kubeseal --controller-name=sealed-secrets --controller-namespace=sealed-secrets -o yaml < mail-secrets-raw.yaml > mail-secrets.yaml
```

