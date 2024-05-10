# Prerequisite
Install hostpath storage for microk8s
```
microk8s enable hostpath-storage
```

# Steps

```
k create -f configmap.yaml
```

```
k create -f persistentvolumeclaim.yaml
```

```
k create configmap sit727-conf-files-config --from-file config
```

```
k create -f deployment.yaml
```