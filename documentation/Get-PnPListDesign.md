---
Module Name: PnP.PowerShell
title: Get-PnPListDesign
schema: 2.0.0
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
online version: https://pnp.github.io/powershell/cmdlets/Get-PnPListDesign.html
---
 
# Get-PnPListDesign

## SYNOPSIS

**Required Permissions**

* SharePoint: Access to the SharePoint Tenant Administration site

Retrieve List Designs that have been registered on the current tenant.

## SYNTAX

```powershell
Get-PnPListDesign [[-Identity] <TenantListDesignPipeBind>] [-Connection <PnPConnection>] [<CommonParameters>]
```

## DESCRIPTION

Retrieve List Designs that have been registered on the current tenant. When providing a name with -Identity, it returns all list designs with that name.

## EXAMPLES

### EXAMPLE 1
```powershell
Get-PnPListDesign
```

Returns all registered list designs

### EXAMPLE 2
```powershell
Get-PnPListDesign -Identity 5c73382d-9643-4aa0-9160-d0cba35e40fd
```
Returns a specific registered list design by id

### EXAMPLE 3
```powershell
Get-PnPListDesign -Identity ListEvent
```

Returns a specific registered list design by name

## PARAMETERS

### -Identity
If specified, it will retrieve the specified list design

```yaml
Type: TenantListDesignPipeBind
Parameter Sets: (All)

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Connection
Optional connection to be used by the cmdlet. Retrieve the value for this parameter by either specifying -ReturnConnection on Connect-PnPOnline or by executing Get-PnPConnection.

```yaml
Type: PnPConnection
Parameter Sets: (All)

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## RELATED LINKS

[Microsoft 365 Patterns and Practices](https://aka.ms/m365pnp)