## Using Azure CLI basic command
### Deploy ARM template with paramter file
```
az vm create --resource-group clement-bonnet-rg --name ubuntu-vm-001 --image Ubuntu2004 --admin-username clem –admin-password mysuperpassword987!
```

## Using Azure CLI and ARM templates
### Deploy ARM template with paramter file
```
az deployment group create --name my-deployment --resource-group clement-bonnet-001-rg --template-file vm.json --parameters vm.parameter.json
```

### Deploy ARM template with inline parameters
```
az deployment group create --name my-deployment --resource-group  clement-bonnet-001-rg --template-file vm.json --parameters vmSize=standard_b1s location=westeurope vmName=ubuntu-vm-001
```
