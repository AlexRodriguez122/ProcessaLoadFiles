---
external help file: ProcessaLoadFiles-help.xml
Module Name: ProcessaLoadFiles
online version: 
schema: 2.0.0
---

# Get-Configuration

## SYNOPSIS
Obtiene la información de los datos de configuración del módulo.

## SYNTAX

```powershell
Get-Configuration
```

## DESCRIPTION
Obtiene la información de los datos de configuración del módulo a partir de los datos en el archivo ProcessaLoadFiles.config

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```powershell
Get-Configuration
```

Obtiene la información de configuración del módulo.

### -------------------------- EXAMPLE 2 --------------------------
```powershell
Get-Configuration | Get-Member -MemberType Properties
```

Obtiene los nombres de las propiedades incluidas en el objeto de retorno.

## PARAMETERS

## INPUTS

### None

## OUTPUTS

### System.Management.Automation.PSObject

## NOTES
Autor: Jarodriguezc

## RELATED LINKS

[[Set-Configuration](Set-Configuration.md)]()

[[Test-Configuration](Test-Configuration.md)]()

