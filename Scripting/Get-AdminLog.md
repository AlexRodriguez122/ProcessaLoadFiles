---
external help file: ProcessaLoadFiles-help.xml
Module Name: ProcessaLoadFiles
online version: 
schema: 2.0.0
---

# Get-AdminLog

## SYNOPSIS
Obtiene el Log que género el proceso de Powershell.

## SYNTAX

### ByProcessId (Default)
```powershell
Get-AdminLog [-ProcessId <Int32>] -InitialDate <DateTime> -FinalDate <DateTime>
```

### ByEmail
```powershell
Get-AdminLog [-Email <String>] -InitialDate <DateTime> -FinalDate <DateTime>
```

## DESCRIPTION
Obtiene el Log que género el proceso de Powershell.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```powershell
Find-BonusLog -BonusNumber 1234567891234567 -ProcessType Cancellation -InitialDate '2017-11-11' -FinalDate '2017-11-13' | Get-AdminLog  -InitialDate '2017-11-11' -FinalDate '2017-11-15'
```

### -------------------------- EXAMPLE 2 --------------------------
```powershell
Get-AdminLog -InitialDate '2017-11-11' -FinalDate '2017-11-15'
```

### -------------------------- EXAMPLE 3 --------------------------
```powershell
Get-AdminLog -InitialDate '2017-11-11' -FinalDate '2017-11-15' -ProcessId 52410
```

## PARAMETERS

### -ProcessId
ProcessId de la ejecución del módulo para una búsqueda exacta.

```yaml
Type: Int32
Parameter Sets: ByProcessId
Aliases: 

Required: False
Position: Named
Default value: 0
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Email
{{Fill Email Description}}

```yaml
Type: String
Parameter Sets: ByEmail
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InitialDate
Fecha inicial de búsqueda del log.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FinalDate
Fecha final de búsqueda del log.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

### System.Management.Automation.PSObject

## NOTES
Autor: Jarodriguezc

## RELATED LINKS

