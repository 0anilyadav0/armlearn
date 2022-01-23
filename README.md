# armlearn

1. https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/parameters
2. New-AzResourceGroupDeployment -Name "deploystorage" -ResourceGroupName "rg01" -TemplateFile .\template.json
3. Parameters : -TemplateParameterObject  
    @parameters = @{
        stgname="azaystg001"
        stgtype="standard_lrs"
    }
4. Functions : https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/template-functions
    a. paramerters()
    b. variables()
    c. concat()
    d. copyIndex()
5. whatif
6. https://docs.microsoft.com/en-us/azure/templates/   -details of each resources
7. New-AzResourceGroupDeployment -Name "deploystorage" -ResourceGroupName "rg01" -TemplateFile template1_empty.json -Mode Complete  - use to detroy and full deployment
8. Test-AzResourceGroupDeployment --- for pre-flight error. other type of error is in-flight error