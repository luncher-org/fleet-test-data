# Helm Example

This example will deploy the `ConfigMap` resource with custom values using `valuesFrom` in `fleet.yaml`.
The `ConfigMap` will be deployed into the `default` namespace.

```yaml
kind: GitRepo
apiVersion: fleet.cattle.io/v1alpha1
metadata:
  name: helm
  namespace: fleet-local
spec:
  repo: https://github.com/rancher/fleet-test-data
  paths:
  - qa-test-apps/helm-app/values-from-with-no-values
```
