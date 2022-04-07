# k8s-jetstack-secure

NOTE! There are resources within this chart that require a custom CRD (keymaker.equinixmetal.com/v1) which is not yet open-sourced. This repo is PURELY AN EXAMPLE and should not be imported / used other than as an example.

At Equinix Metal we use helm primarily for variable inheritance with Argo CD. This is why you will see empty values in the `values.yaml` - when we template out our Argo applications the variables around the cluster components are running on are generated in those applications. This allows us to deploy a single chart globally but pass in templated variables.

The Jetstack Agent is an open source [project](https://github.com/jetstack/jetstack-secure) and the agent deployment yaml (it's linked far down the page and there's no anchors) can be found [here](https://platform.jetstack.io/docs/google-cloud-marketplace).
