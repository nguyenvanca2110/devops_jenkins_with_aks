## Access Azure Kubernetes Cluster from Local Machine. 
## Install Azure CLI
```sh

## Download & Install Azure CLI on Windows
https://aka.ms/installazurecliwindows
```

## Once download is complete, Install .msi file to get azure cli
```sh
Open CMD
type az --help --> to test whether Azure CLI is installed correctly or not
```
## Once Installation is completed, need to Access Azure with below commands
```sh
# Login with Azure credentials 
az login
# Incase we have multiple subscriptions
az account set --subscription <SubscriptionName> 

#  Get the credentials of AKS in local to mange the Cluster 
az aks get-credentials --resource-group=<RGNAME> --name=<AKSCLUSTERNAME>

# After this step we have
# Merged "AKSCLUSTERNAME" as current context in /root/.kube/config
```
## Install kubectl command line package in Local Windows Machine
```sh
curl -LO https://dl.k8s.io/release/v1.22.0/bin/windows/amd64/kubectl.exe
```

