---
title: "Multi-dimensional array cannot be converted to an expression tree"
ms.custom: na
ms.date: 10/01/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 65eefab7-c7ad-4dcd-bebf-2d16fba9f28f
caps.latest.revision: 6
manager: douge
translation.priority.ht: 
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - ru-ru
  - zh-cn
  - zh-tw
translation.priority.mt: 
  - cs-cz
  - pl-pl
  - pt-br
  - tr-tr
---
# Multi-dimensional array cannot be converted to an expression tree
Most expressions can be converted to expression trees, but multi-dimensional arrays cannot be. For example, the following code causes this error:  
  
```vb#  
Module Module1  
    Sub Main()  
        '' A multi-dimensional array cannot be converted.  
        'Dim expTree As Expressions.Expression(Of Func(Of Object)) = _  
        '    Function() New Integer(1, 1) {{1, 2}, {2, 3}}  
  
        ' A one-dimensional array can be converted.  
        Dim expTree2 As Expressions.Expression(Of Func(Of Object)) = _  
            Function() New Integer() {1, 2, 3}  
    End Sub  
End Module  
```  
  
 **Error ID:** BC36603  
  
## See Also  
 [NOT IN BUILD: Expression Trees in LINQ](assetId:///1a2e8e74-4bbc-45ab-9a46-2b6cfce3bcb2)   
 [How to: Use Expression Trees to Build Dynamic Queries](../Topic/How%20to:%20Use%20Expression%20Trees%20to%20Build%20Dynamic%20Queries%20\(C%23%20and%20Visual%20Basic\).md)   
 [NOTINBUILD Multidimensional Arrays in Visual Basic](assetId:///d92cad25-07e2-4d79-8ea4-ab269700f5de)