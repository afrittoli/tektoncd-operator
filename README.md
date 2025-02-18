# Tektoncd Operator

The quickest and easiest way to install, upgrade and manage TektonCD [Pipelines](https://github.com/tektoncd/pipeline),
[Dashboard](https://github.com/tektoncd/dashboard), [Triggers](https://github.com/tektoncd/triggers)
on any Kubernetes Cluster.


# Quick Start

## Install Tektoncd Operator

1. Install operator
    ```
    $ kubectl apply -f https://storage.googleapis.com/tekton-releases/operator/latest/release.yaml
    ```
1. Install Components (uses [installation profiles](https://github.com/tektoncd/operator/tree/main/config/crs/kubernetes/config): `default`, `all`, `basic`)
    ```
    # to installl pipelines, triggers and dashboard (use profile 'all')
    $ kubectl apply -f https://raw.githubusercontent.com/tektoncd/operator/main/config/crs/kubernetes/config/all/operator_v1alpha1_config_cr.yaml
    ```

# References

- [Development Guide](docs/README.md)
- [Testing Guide](test/README.md)

### Read the docs

| Version | Docs |
| ------- | ---- |
| [HEAD](/README.md) | [Docs @ HEAD](/docs/README.md) |
| [v0.21.0-1](https://github.com/tektoncd/operator/releases/tag/v0.21.0-1) | [Docs @ v0.21.0-1](https://github.com/tektoncd/operator/tree/v0.21.0-1/docs) | [Examples @ v0.21.0](https://github.com/tektoncd/pipeline/tree/v0.21.0/examples#examples) |
