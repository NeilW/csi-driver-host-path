# Kustomize Namespace

This directory has a basic `kustomization.yaml` file to allow you to run
the host-path driver in a separate namespace - all without editing a file!

## To use
- Copy the entire directory to a directory on the machine where `kubectl` can access your cluster
- Make the changes you wish to the base versions and the namespace name.
- Apply the directory with `kubectl apply -k <directory name>`

## To change images
- Uncomment the images line you require and alter the version of the
component to the one you want to test.

## For more details
See the [help document](https://kubectl.docs.kubernetes.io/pages/reference/kustomize.html) for the kustomization.yaml
