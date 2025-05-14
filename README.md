# spring-petclinic-virt

1. Create new namespace (e.g: sample)
2. Deploy mysql-vm.yaml first and take note of VMs IP.
3. Change the following line of web-vm.yaml:

```
Environment="MYSQL_URL=jdbc:mysql://10.135.0.63:3306/petclinic" # CHANGE IP TO MYSQL
```

4. Deploy web-*.yaml
