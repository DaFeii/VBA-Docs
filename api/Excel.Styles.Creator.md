---
title: Styles.Creator property (Excel)
keywords: vbaxl10.chm178074
f1_keywords:
- vbaxl10.chm178074
api_name:
- Excel.Styles.Creator
ms.assetid: 4ca8554c-8acb-8715-c13c-456cb7c255e0
ms.date: 05/16/2019
ms.localizationpriority: medium
---


# Styles.Creator property (Excel)

Returns a 32-bit integer that indicates the application in which this object was created. Read-only **Long**.


## Syntax

_expression_.**Creator**

_expression_ A variable that represents a **[Styles](Excel.Styles.md)** object.


## Remarks

If the object was created in Microsoft Excel, this property returns the string XCEL, which is equivalent to the hexadecimal number 5843454C. The **Creator** property is designed to be used in Microsoft Excel for the Macintosh, where each application has a four-character creator code. For example, Microsoft Excel has the creator code XCEL.




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]