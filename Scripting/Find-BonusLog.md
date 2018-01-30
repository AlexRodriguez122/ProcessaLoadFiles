---
external help file: ProcessaLoadFiles-help.xml
Module Name: ProcessaLoadFiles
online version: 
schema: 2.0.0
---

# Find-BonusLog

## SYNOPSIS
Encuentra el bono en el archivo de log que se envió al cliente y el processid del Powershell que lo ejecuto.

## SYNTAX

### WithDateRange
```powershell
Find-BonusLog -BonusNumber <Int64> -ProcessType <String> -InitialDate <DateTime> -FinalDate <DateTime>
```

### OnlyBonusNumber
```powershell
Find-BonusLog -BonusNumber <Int64> -ProcessType <String>
```

## DESCRIPTION
Encuentra el bono en el archivo de log que se envió al cliente y el processid del Powershell que lo ejecuto.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```powershell
Find-BonusLog -BonusNumber 1234567891234567 -ProcessType Activation
```

### -------------------------- EXAMPLE 2 --------------------------
```powershell
Find-BonusLog -BonusNumber 1234567891234567 -ProcessType Activation -InitialDate '2017-11-11' -FinalDate '2017-11-13'
```

## PARAMETERS

### -BonusNumber
Número del bono que se desea encontrar.

```yaml
Type: Int64
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProcessType
Proceso que se realizó con el número del bono.
(Activación, Cancelación o Bloqueo).

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InitialDate
Fecha inicial de búsqueda del log y el idprocess.

```yaml
Type: DateTime
Parameter Sets: WithDateRange
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FinalDate
Fecha final de búsqueda del log y el idprocess.

```yaml
Type: DateTime
Parameter Sets: WithDateRange
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

