test for CICD
test for Automating Docker Deployments to Azure with GitHub Actions


Your App has been deployed at: 
http://myappdeployment.canadacentral.azurecontainer.io:3000/

How to solve:
```
Error: Error: The client '' with object id '' does not have authorization to perform action 'Microsoft.ContainerInstance/containerGroups/write' over scope '/subscriptions/xxx/resourceGroups/xxx/providers/Microsoft.ContainerInstance/containerGroups/xxx' or the scope is invalid. If access was recently granted, please refresh your credentials.

```

```
az role assignment create --assignee <service-principal-client-id> --role Owner --scope /subscriptions/<subscription-id>/resourceGroups/<resource-group-name>
```