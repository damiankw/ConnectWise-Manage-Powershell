# Remove-CWMCompanyConfiguration
## SYNOPSIS
This function will remove a company configuration from Manage.
## SYNTAX
```powershell
Remove-CWMCompanyConfiguration [[-CompanyConfigurationID] <Int32>] [<CommonParameters>]
```
## PARAMETERS
### -CompanyConfigurationID &lt;Int32&gt;

```
Required                    false
Position                    1
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

https://developer.connectwise.com/manage/rest?a=Company&e=Configurations&o=DELETE
