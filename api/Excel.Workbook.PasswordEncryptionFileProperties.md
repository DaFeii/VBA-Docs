---
title: Workbook.PasswordEncryptionFileProperties property (Excel)
keywords: vbaxl10.chm199215
f1_keywords:
- vbaxl10.chm199215
api_name:
- Excel.Workbook.PasswordEncryptionFileProperties
ms.assetid: 536ad729-424e-5f81-85e9-8a6ed71fb11a
ms.date: 05/29/2019
ms.localizationpriority: medium
---


# Workbook.PasswordEncryptionFileProperties property (Excel)

**True** if Microsoft Excel encrypts file properties for the specified password-protected workbook. Read-only **Boolean**.


## Syntax

_expression_.**PasswordEncryptionFileProperties**

_expression_ A variable that represents a **[Workbook](Excel.Workbook.md)** object.


## Remarks

Use the **[SetPasswordEncryptionOptions](Excel.Workbook.SetPasswordEncryptionOptions.md)** method to specify whether Excel encrypts file properties for the specified password-protected workbook.


## Example

This example sets the password encryption options if the file properties are not encrypted for password-protected workbooks.

```vb
Sub SetPasswordOptions() 
 
 With ActiveWorkbook 
 If .PasswordEncryptionFileProperties = False Then 
 .SetPasswordEncryptionOptions _ 
 PasswordEncryptionProvider:="Microsoft RSA SChannel Cryptographic Provider", _ 
 PasswordEncryptionAlgorithm:="RC4", _ 
 PasswordEncryptionKeyLength:=56, _ 
 PasswordEncryptionFileProperties:=True 
 End If 
 End With 
 
End Sub
```



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]