# Workadventure on Kubernetes

This Helm chart deploys [Workadventure](https://github.com/workadventure/workadventure) on Kubernetes.

It is an adaptation of the [official Docker Compose deployment](https://github.com/workadventure/workadventure/tree/master/contrib/docker).

## Configuration

Since the original Container images are completely configured via environment variables, this Helm chart have to use the same approach. Theres is a corresponding `xxx-secret-env.yaml` file and a `xxx-env.yaml` file, which contains all environments variables. Additional entries can be easely added in the corresponding sections in the values file.

There are the `commonEnv` and `commonSecretEnv` sections, which are used in all services.

Please the original [Dokumentation](https://github.com/workadventure/workadventure/blob/master/contrib/docker/docker-compose.prod.yaml) for reference.
