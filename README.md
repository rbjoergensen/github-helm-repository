# GitHub Helm Repository
Hosting a Helm repository in GitHub using pages.

## Todo
- Versioning
- Linting

## Usage
[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

  helm repo add rbjoergensen https://rbjoergensen.github.io/github-helm-repository

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
<alias>` to see the charts.

To install the <chart-name> chart:

    helm install rbjoergensen-test-chart rbjoergensen/nginx

To uninstall the chart:

    helm delete rbjoergensen-test-chart

## Links

- https://helm.sh/docs/howto/chart_releaser_action/
- https://github.com/helm/chart-releaser-action
- https://helm.sh/docs/topics/chart_repository/
- https://www.harness.io/blog/helm-chart-repo