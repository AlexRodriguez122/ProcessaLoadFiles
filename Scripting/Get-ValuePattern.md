---
external help file: ProcessaLoadFiles-help.xml
Module Name: ProcessaLoadFiles
online version: 
schema: 2.0.0
---

# Get-ValuePattern

## SYNOPSIS
Obtiene información según la expresión regular y el archivo indicados.

## SYNTAX

```powershell
Get-ValuePattern [-FilePath] <String> [-Regex] <String> [[-EmailFrom] <String>] [-LogPath] <String>
```

## DESCRIPTION
Obtiene información según la expresión regular y el archivo indicados.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```powershell
Get-ValuePattern -FilePath 'c:\Ruta.txt' -LogPath 'c:\Ruta_Log.txt' -Regex '[0-9]{16}'
```

## PARAMETERS

### -FilePath
Ruta completa del Archivo.

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

### -Regex
Expresión regular con la cual se obtendrá la información del archivo.

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

### -EmailFrom
{{Fill EmailFrom Description}}

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LogPath
Ruta del log en el cual se está guardando la información.

```yaml
Type: String
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

### System.String[]

## NOTES
Autor: Jarodriguezc

## RELATED LINKS

