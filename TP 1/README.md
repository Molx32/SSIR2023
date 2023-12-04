### Deploy ARM template with paramter file
```
az deployment group create --name my-deployment --resource-group clement-bonnet-001-rg --template-file vm.json --parameters vm.parameter.json
```

### Deploy ARM template with inline parameters
```
az deployment group create --name my-deployment --resource-group  clement-bonnet-001-rg --template-file vm.json --parameters vmSize=standard_b1s location=westeurope vmName=ubuntu-vm-001
```
