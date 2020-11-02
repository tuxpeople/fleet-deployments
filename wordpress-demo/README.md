# Speed-Test Plotter deployment

This example will deploy the [Speedtest-Plotter](https://github.com/ansemjo/speedtest-plotter) application with my own image and configured with PV and a specific server.
The app will be deployed into the `default` namespace.

```yaml
kind: GitRepo
apiVersion: fleet.cattle.io/v1alpha1
metadata:
  name: speedtest-plotter
  namespace: fleet-default
spec:
  branch: main
  repo: https://github.com/tuxpeople/fleet-deployments
  paths:
  - wordpress-demo
```
