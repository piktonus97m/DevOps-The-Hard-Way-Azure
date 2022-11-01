# Connecting To Elastic Kubernetes Service (AKS)

When you're deploying locally, without any CI/CD to AKS, you'll need to authenticate from your local terminal.

Once you authenticate to AKS from your local terminal, a `kubeconfig` gets stored on your computer. The `kubeconfig` has all of the connection information and authentication needs to connect to AKS.

## Connecting To AKS

1. Run the following command to connect to AKS:
`az aks get-credentials --resource-group rropemike-rg --name rropemikeaks` > In order to login without any issues please use the --admin tag[. Please reference to the following link ](https://chamindac.blogspot.com/2022/09/resolve-unable-to-connect-to-server.html)


2. Once connected, you should be able to run commands like the following to confirm you're connected:
`kubectl get nodes`
