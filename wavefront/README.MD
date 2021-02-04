To Depoly Wavefront Proxy to your new cluster

#### Step 1 ####

Create a namespace for the proxy

```
kubectl create namespace wavefront 
```

#### Step 3 ####

Setup RBAC in the new namespace

'''
kubectl apply -f to-rbac.yaml -n wavefront
'''

#### Step 2 ####
Use Helm to insall the proxy

Note: remember to add the wavefront repo and update

```
helm install wavefront wavefront/wavefront  --set wavefront.url=https://longboard.wavefront.com  --set wavefront.token=YOUR TOKEN --set clusterName="YOUR CLUSTER" --namespace wavefront
```

#### Step 1 ####
#### Step 1 ####
#### Step 1 ####
#### Step 1 ####
#### Step 1 ####
