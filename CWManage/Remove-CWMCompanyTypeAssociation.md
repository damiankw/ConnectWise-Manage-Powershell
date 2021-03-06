# Remove-CWMCompanyTypeAssociation
## SYNOPSIS
This function will remove a type from a company.
## SYNTAX
```powershell
Remove-CWMCompanyTypeAssociation [-CompanyID] <Int32> [-TypeAssociationID] <Int32> [<CommonParameters>]
```
## PARAMETERS
### -CompanyID &lt;Int32&gt;
The ID of the company configuration that you want to delete.
```
Required                    true
Position                    1
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -TypeAssociationID &lt;Int32&gt;
The ID of the company configuration that you want to delete.
```
Required                    true
Position                    2
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
## EXAMPLES
### EXAMPLE 1
```powershell
PS C:\>Remove-CWMCompanyConfiguration -CompanyConfigurationID 123
```

## NOTES
Author: Chris Taylor

Date: 7/3/2017 
## LINKS
http://labtechconsulting.com

https://developer.connectwise.com/Products/Manage/REST?a=Company&e=CompanyCompanyTypeAssociations&o=DELETE
