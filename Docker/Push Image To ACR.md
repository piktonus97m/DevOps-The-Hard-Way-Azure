# Push Image To ACR

The ACR repo will be where you store the Docker image that you created on your local computer in step 2.

## Log Into The ACR Repository
1. Log in to ACR with Azure CLI
`az acr login --name rropemikeacr`


## Tag The Docker image
1. Tag the Docker image
`docker tag uberapp rropemikeacr.azurecr.io/uberapp:v1`

## Push The Docker Image To ACR
1. Push the Docker image to ACR
`docker push rropemikeacr.azurecr.io/uberapp:v1`
