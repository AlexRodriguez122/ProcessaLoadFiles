---
external help file: ProcessaLoadFiles-help.xml
Module Name: ProcessaLoadFiles
online version: 
schema: 2.0.0
---

# Invoke-BonusCancellation

## SYNOPSIS
Realiza la cancelación de los bonos encontrados en un archivo.

## SYNTAX

```powershell
Invoke-BonusCancellation [-FilePath] <String> [-EmailFrom] <String> [-Subject] <String> [-EmailDate] <DateTime>
```

## DESCRIPTION
Cancela los bonos encontrados con una expresión regular en un archivo indicado.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```powershell
Invoke-BonusCancellation -FilePath 'C:\Ruta\Archivo.txt' -EmailFrom 'Correo@Correo.com' -Subject 'asunto Correo' -EmailDate (Get-Date)
```

### -------------------------- EXAMPLE 2 --------------------------
```powershell
Invoke-BonusCancellation -FilePath 'C:\Ruta\Archivo.txt' -EmailFrom 'Correo@Correo.com' -Subject 'asunto Correo' -EmailDate '2017-07-07'
```

## PARAMETERS

### -FilePath
Ruta del archivo que contiene los números de bono para realizar la cancelación.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EmailFrom
Correo o Correos electrónicos de los cuales fue recibido el correo.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Subject
Asunto del correo electrónico con el cual se recibio el correo.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EmailDate
Fecha en que el correo fue recibido.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: True
Position: 4
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

