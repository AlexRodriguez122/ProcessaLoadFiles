---
external help file: ProcessaLoadFiles-help.xml
Module Name: ProcessaLoadFiles
online version: 
schema: 2.0.0
---

# Test-Configuration

## SYNOPSIS
Verifica la información de los datos de configuración del módulo.

## SYNTAX

```powershell
Test-Configuration [-SaveFlag]
```

## DESCRIPTION
Verifica la información de los datos de configuración en el archivo PSJobMonitor.config.
Se genera una excepción si falla alguna comprobación.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```powershell
Test-Configuration -Verbose
```

Verifica la configuración del módulo y muestra mensajes en pantalla de cada validación.

## PARAMETERS

### -SaveFlag
Si está presente, se guardará la configuración.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

### Ninguno.

## OUTPUTS

### System.Void

## NOTES
Autor: Jarodriguezc

## RELATED LINKS

[[Set-Configuration](Set-Configuration.md)]()

[[Get-Configuration](Get-Configuration.md)]()

