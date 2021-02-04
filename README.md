# Istio Helm Charts

This repository contains the source files of some of the Istio charts published at https://github.com/istio/istio. You can download the latest version of the charts following [these instructions](https://istio.io/latest/docs/setup/getting-started/#download). 

The follow instructions will guide you in updating the charts in this repository (or adding new ones):

1. Go in the root directory
1. Copy the chart(s) in `sources/` preserving the original directory structure (i.e. the one in the .zip file downloaded from Istio, see above)
1. Run `helm package sources/*` to package all the charts
1. Run `helm repo index --url https://kynetics.github.io/istio-helm-charts/ --merge index.yaml .` to re-generate the `index.yaml` file
1. Commit and push
