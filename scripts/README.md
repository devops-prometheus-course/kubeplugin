# kubeplugin

# Deploy the Metrics Server with the following command:
```sh
kubectl apply -f https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml
```

# "Install" plugin by moving it to a directory in your $PATH
```sh
sudo mv ./kubeplugin /usr/local/bin
```

# Check that kubectl recognizes plugin:
```sh
kubectl plugin list
```

# Now check plugin with example below:
```sh
kubectl kubeplugin <namespace> <kubectl_operation> <resource_type>
```