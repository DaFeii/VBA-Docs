---
title: PivotField.AutoSortField property (Excel)
keywords: vbaxl10.chm240114
f1_keywords:
- vbaxl10.chm240114
api_name:
- Excel.PivotField.AutoSortField
ms.assetid: f31499e6-dea7-5e54-2316-9088bd5670b3
ms.date: 05/04/2019
ms.localizationpriority: medium
---


# PivotField.AutoSortField property (Excel)

Returns the name of the data field used to sort the specified PivotTable field automatically. Read-only **String**.


## Syntax

_expression_.**AutoSortField**

_expression_ A variable that represents a **[PivotField](Excel.PivotField.md)** object.


## Example

This example displays a message box showing the **AutoSort** parameters for the Product field.

```vb
With Worksheets(1).PivotTables(1).PivotFields("product") 
 Select Case .AutoSortOrder 
 Case xlManual 
 aso = "manual" 
 Case xlAscending 
 aso = "ascending" 
 Case xlDescending 
 aso = "descending" 
 End Select 
 MsgBox " sorted in " & aso & _ 
 " order by " & .AutoSortField 
End With
```




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]