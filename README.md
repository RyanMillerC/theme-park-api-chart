**NOTE: This repo is part of [Hello OpenShift: Multi-Cluster GitOps].** It's
not intended to be referenced directly. Instead, check out the organization's
page for how this repository fits into the greater multi-cluster GitOps
architecture.

# Theme Park API - Helm Charts

This repo contains 3 example Helm charts to deploy REST APIs that serve roller
coaster data from 3 theme parks in the greater Washington D.C. area: Hershey
Park, Kings Dominion, and Six Flags. It's used as an example of how
applications could be structured and deployed through the multi-cluster GitOps
reference architecture.

Each chart has 4 environments, *Dev*, *Test*, *Stage*, and *UAT*. Dev and Test
are deployed to the Dev cluster. Stage and UAT are deployed to the Stage
cluster.

Each environment has it's own values.yaml file. All environments are
deployed to OpenShift through OpenShift GitOps (Argo CD). The Argo CD
configurations to deploy these charts are in [gitops-dev] and [gitops-stage]
respectively.

[Hello OpenShift: Multi-Cluster GitOps]: https://github.com/hello-openshift-multicluster-gitops
[gitops-dev]: https://github.com/hello-openshift-multicluster-gitops/gitops-dev
[gitops-stage]: https://github.com/hello-openshift-multicluster-gitops/gitops-stage
