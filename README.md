Credits to https://github.com/cloudecho/charts

## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

  helm repo add cloudecho https://cloudecho.github.io/charts

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
cloudecho` to see the charts.

To install the hello chart:

    helm install my-hello cloudecho/hello

To uninstall the chart:

    helm delete my-hello


## Build

Build chart repo:

```
git checkout gh-pages
make
```# chart-hello-world
