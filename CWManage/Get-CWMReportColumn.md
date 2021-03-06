# Get-CWMReportColumn
## SYNOPSIS
This function will list the columns of the specified report.
## SYNTAX
```powershell
Get-CWMReportColumn [-Report] <String> [<CommonParameters>]
```
## PARAMETERS
### -Report &lt;String&gt;
The name of the report you want the columns for.
```
Required                    true
Position                    1
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
## EXAMPLES
### EXAMPLE 1
```powershell
PS C:\>Get-CWMReportColumn -Report ServiceNote

Will return columns for the ServiceNote report.
```

## NOTES
Author: Chris Taylor

Date: 11/12/2018 
## LINKS
http://labtechconsulting.com

https://developer.connectwise.com/products/manage/rest?a=System&e=Reports&o=COLUMNS
