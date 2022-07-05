# chart-sample

Repository used to test some behavior with a dummy public chart

# Usage

## Package helm chart

```console
helm package sample --version 0.2.0

```

## Upload package to Releases
```console
cr upload --owner Feggah --git-repo chart-sample --token 12345 --package-path .
```

> Install cr [here](https://github.com/helm/chart-releaser).

## Install helm chart

```console
helm install sample https://github.com/Feggah/chart-sample/releases/download/sample-0.2.0/sample-0.2.0.tgz
```
