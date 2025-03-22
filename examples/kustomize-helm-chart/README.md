# Rationale

I am preserving this here, as it was a challenge to come up with, but
will probably never use. This is the most analogous to how I
structured my Flux CD repository:
* installation of a Helm chart
* using base/global values and resources
* with site specific values and resources which override
* with kustomizations.yaml files that explicity lists the resources (manifests)

For an analogous Flux CD example, here is the site specific [kustomizations.yaml](https://github.com/fluxcd/flux2-kustomize-helm-example/blob/main/apps/production/kustomization.yaml) file,
pointing to the base layer [resources](https://github.com/fluxcd/flux2-kustomize-helm-example/tree/main/apps/base/podinfo).
