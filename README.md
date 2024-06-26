# Excel2JSON.ps1

## SYNOPSIS
Converts an Excel sheet from a workbook to JSON

## SYNTAX

```
Excel2JSON.ps1 [-InputFile] <Object> [[-OutputFileName] <String>] [[-SheetName] <String>] [[-$HeaderRow] <Int>] [[-$DetailRow] <Int>]
```

## DESCRIPTION
To allow for parsing of Excel Workbooks suitably in PowerShell, this script converts a sheet from a spreadsheet into a JSON file of the same structure as the sheet.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Excel2JSON.ps1 -InputFile MyExcelWorkbook.xlsx
```

### -------------------------- EXAMPLE 2 --------------------------
```
Get-Item MyExcelWorkbook.xlsx | Excel2JSON.ps1 -OutputFileName MyConvertedFile.json -SheetName Sheet2 -HeaderRow 2 -DetailRow 3
```

## PARAMETERS

### -InputFile
The Excel Workbook to be converted.
Can be FileInfo or a String.

```yaml
Type: Object
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -OutputFileName
The path to a JSON file to be created.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SheetName
The name of the sheet from the Excel Workbook to convert.
If only one sheet exists, it will convert that one.

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
### -HeaderRow
Specifies the row number containing the header in the Excel Workbook.

```yaml
Type: Int
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DetailRow
Specifies the row number containing the detail data in the Excel Workbook.

```yaml
Type: Int
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES
This code was based on the original written by: [Chris Brown](https://github.com/chrisbrownie/Convert-ExcelSheetToJson)

Find me on:
* [My blog](https://blacktdn.com.br/)
* [Github](https://github.com/naldodj)
* [Linkedin](https://www.linkedin.com/in/marinaldo-de-jesus-66392346/)

## RELATED LINKS

* [WIN-PS2EXE](https://github.com/MScholtes/PS2EXE)

* [BlackTDN :: Convertendo Planilha Excel em JSON (Parte I)](https://www.blacktdn.com.br/2024/05/blacktdn-convertendo-planilha-excel-em.html)

