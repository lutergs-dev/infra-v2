### Secrets in ente-photo

maintain secret values needs to use in ente photos.

copy-paste `ente-secret-raw-example.yaml` to `ente-secret-raw.yaml`, and fill out data by given instruction.

!! please remind do not post original `ente-secret-raw.yaml` to git.

and create sealed-secret via execute this command.

```shell
kubeseal --controller-name=sealed-secrets --controller-namespace=sealed-secrets -o yaml < ente-secret-raw.yaml > ente-secret.yaml
```


### Secrets in PostgreSQL

maintain username and password for postgresql

copy-paste `postgresql-secret-raw-example.yaml` to `postgresql-secret-raw.yaml`, and fill out data by given instruction.

!! please remind do not post original `postgresql-secret-raw.yaml` to git.

and create sealed-secret via execute this command.

```shell
kubeseal --controller-name=sealed-secrets --controller-namespace=sealed-secrets -o yaml < postgresql-secret-raw.yaml > postgresql-secret.yaml
```


### Secrets in S3

maintain username and password for S3

copy-paste `s3-secret-raw-example.yaml` to `s3-secret-raw.yaml`, and fill out data by given instruction.

!! please remind do not post original `s3-secret-raw.yaml` to git.

and create sealed-secret via execute this command.

```shell
kubeseal --controller-name=sealed-secrets --controller-namespace=sealed-secrets -o yaml < s3-secret-raw.yaml > s3-secret.yaml
```

