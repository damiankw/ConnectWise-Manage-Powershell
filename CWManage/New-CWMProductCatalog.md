# New-CWMProductCatalog
## SYNOPSIS
This function will create a new catalog.
## SYNTAX
```powershell
New-CWMProductCatalog [-identifier] <String> [-description] <String> [[-inactiveFlag] <Boolean>] [-subcategory] <Object> [-type] <Object> [[-productClass] <String>] [[-serializedFlag] <Boolean>] [[-serializedCostFlag] <Boolean>] [[-phaseProductFlag] <Boolean>] [[-unitOfMeasure] <Object>] [[-minStockLevel] <Int32>] [[-price] <Single>] [[-cost] <Single>] [[-priceAttribute] <Int32>] [[-taxableFlag] <Boolean>] [-customerDescription] <String> [[-manufacturer] <Object>] [[-manufacturerPartNumber] 

<String>] [[-vendor] <Object>] [[-vendorSku] <String>] [[-notes] <String>] [[-integrationXRef] <String>] [[-dateEntered] <String>] [[-category] <Object>] [[-_info] <Object>] [[-customFields] <Object>] [<CommonParameters>]
```
## PARAMETERS
### -identifier &lt;String&gt;

```
Required                    true
Position                    1
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -description &lt;String&gt;

```
Required                    true
Position                    2
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -inactiveFlag &lt;Boolean&gt;

```
Required                    false
Position                    3
Default value                False
Accept pipeline input       false
Accept wildcard characters  false
```
### -subcategory &lt;Object&gt;

```
Required                    true
Position                    4
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -type &lt;Object&gt;

```
Required                    true
Position                    5
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -productClass &lt;String&gt;

```
Required                    false
Position                    6
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -serializedFlag &lt;Boolean&gt;

```
Required                    false
Position                    7
Default value                False
Accept pipeline input       false
Accept wildcard characters  false
```
### -serializedCostFlag &lt;Boolean&gt;

```
Required                    false
Position                    8
Default value                False
Accept pipeline input       false
Accept wildcard characters  false
```
### -phaseProductFlag &lt;Boolean&gt;

```
Required                    false
Position                    9
Default value                False
Accept pipeline input       false
Accept wildcard characters  false
```
### -unitOfMeasure &lt;Object&gt;

```
Required                    false
Position                    10
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -minStockLevel &lt;Int32&gt;

```
Required                    false
Position                    11
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -price &lt;Single&gt;

```
Required                    false
Position                    12
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -cost &lt;Single&gt;

```
Required                    false
Position                    13
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -priceAttribute &lt;Int32&gt;

```
Required                    false
Position                    14
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -taxableFlag &lt;Boolean&gt;

```
Required                    false
Position                    15
Default value                False
Accept pipeline input       false
Accept wildcard characters  false
```
### -customerDescription &lt;String&gt;

```
Required                    true
Position                    16
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -manufacturer &lt;Object&gt;

```
Required                    false
Position                    17
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -manufacturerPartNumber &lt;String&gt;

```
Required                    false
Position                    18
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -vendor &lt;Object&gt;

```
Required                    false
Position                    19
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -vendorSku &lt;String&gt;

```
Required                    false
Position                    20
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -notes &lt;String&gt;

```
Required                    false
Position                    21
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -integrationXRef &lt;String&gt;

```
Required                    false
Position                    22
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -dateEntered &lt;String&gt;

```
Required                    false
Position                    23
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -category &lt;Object&gt;

```
Required                    false
Position                    24
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -_info &lt;Object&gt;

```
Required                    false
Position                    25
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -customFields &lt;Object&gt;

```
Required                    false
Position                    26
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
## EXAMPLES
### EXAMPLE 1
```powershell
PS C:\>$Catalog = @{

'identifier' = $Product.offerName
    'description' = $Product.offerName
    'subcategory' = @{id = 152}
    'type' = @{id = 47}
    'customerDescription' = $Product.offerName
    'cost' = $Product.unitPrice
    'price' = $Price
    'manufacturerPartNumber' = $Product.offerName
    'manufacturer' = $Manufacturer
    'productClass' = 'Agreement'
    'taxableFlag' = $true
}
New-CWMCatalog @Catalog
```

## NOTES
Author: Chris Taylor

Date: 10/10/2018 
## LINKS
http://labtechconsulting.com

https://developer.connectwise.com/manage/rest?a=Procurement&e=CatalogsItem&o=CREATE
