# tkn

This task performs operations on Tekton resources using
[`tkn`](https://github.com/tektoncd/cli).

This task performs operations with KubeVirt resources using [`virtctl`](https://github.com/kubevirt/kubevirt)

## Install the Task

```
kubectl apply -f https://raw.githubusercontent.com/tektoncd/catalog/master/task/virtctl/0.1/virtctl.yaml
```

## Parameters

name      | description                                 | default
--------- | ------------------------------------------- | -------
virtctl-image | `virtctl` CLI container image to run this task. | quay.io/my-org/virtctl:latest
ARGS      | The arguments to pass to the `virtctl` CLI.     | No default. Required.
