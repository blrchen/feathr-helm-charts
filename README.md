# feathr-helm-charts

## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

```bash
helm repo add feathr-helm-charts https://blrchen.github.io/feathr-helm-charts
```

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
feathr-online-server` to see the charts.

To install the feathr-online-server chart:

```bash
helm install feathr-online-server feathr-helm-charts/feathr-online-server
```

To uninstall the chart:

```bash
helm delete feathr-online-server
```

## Local Development

To test changes to the chart locally, run the following command from the directory /charts

```bash
helm install feathr-online-server ./feathr-online-server -f ./feathr-online-server/values.yaml
```
