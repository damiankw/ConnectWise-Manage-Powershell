# Update-CWMProjectPhase
## SYNOPSIS
This will update an project phase.
## SYNTAX
```powershell
Update-CWMProjectPhase [-ProjectID] <Object> [-PhaseID] <Object> [-Operation] <Object> [-Path] <String> [-Value] <String> [<CommonParameters>]
```
## PARAMETERS
### -ProjectID &lt;Object&gt;
The ID of the project that you are updating. List-CWProjects
```
Required                    true
Position                    1
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -PhaseID &lt;Object&gt;
The ID of the phase that you are updating. Get-CWProjectPhases
```
Required                    true
Position                    2
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -Operation &lt;Object&gt;
What you are doing with the value. 

replace
```
Required                    true
Position                    3
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -Path &lt;String&gt;
The value that you want to perform the operation on.
```
Required                    true
Position                    4
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -Value &lt;String&gt;
The value of that operation.
```
Required                    true
Position                    5
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
## EXAMPLES
### EXAMPLE 1
```powershell
PS C:\>$UpdateParam = @{

ProjectID = $Project.id
    PhaseID = $Phase.id
    Operation = 'replace'
    Path = 'status'
    Value = $Value
}
Update-CWProjectPhase @UpdateParam
```

## NOTES
Author: Chris Taylor

Date: 10/10/2018 
## LINKS
http://labtechconsulting.com

https://developer.connectwise.com/products/manage/rest?a=Project&e=ProjectPhases&o=UPDATE
