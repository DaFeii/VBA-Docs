---
title: Include property (Excel Graph)
keywords: vbagr10.chm65701
f1_keywords:
- vbagr10.chm65701
api_name:
- Excel.Include
ms.assetid: ed92c49d-88fc-7f44-15cf-0641032157b2
ms.date: 04/11/2019
ms.localizationpriority: medium
---


# Include property (Excel Graph)

**True** if the data in the specified row or column is included in the chart. Read/write **Variant**.

## Syntax

_expression_.**Include**

_expression_ Required. An expression that returns one of the objects in the **Applies To** list.


## Example

This example causes the data in the second row on the datasheet to be excluded from the chart.

```vb
With myChart.Application.DataSheet 
 .Rows(2).Include = False 
End With
```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]