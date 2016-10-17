---
title: "Constraint &#39;&lt;constraint1&gt;&#39; conflicts with the constraint &#39;&lt;constraint2&gt;&#39; already specified for type parameter &#39;&lt;typeparametername&gt;&#39;"
ms.custom: na
ms.date: 10/01/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 30e6778d-5c2b-4f2d-a136-4e66fa9fbe4d
caps.latest.revision: 8
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
# Constraint &#39;&lt;constraint1&gt;&#39; conflicts with the constraint &#39;&lt;constraint2&gt;&#39; already specified for type parameter &#39;&lt;typeparametername&gt;&#39;
A generic type is declared with conflicting constraints on a type parameter.  
  
 The following statement can generate this error.  
  
 `Public Class testClass(Of t As {Structure, Class })`  
  
 The constraints `Structure` and `Class` cause a conflict for type parameter `t`, because the `Structure` constraint requires that the corresponding type argument be a value type, while `Class` requires that it be a reference type.  
  
 **Error ID:** BC32119  
  
### To correct this error  
  
-   Change the type parameter constraints to avoid conflicts.  
  
## See Also  
 [Generic Types in Visual Basic](../Topic/Generic%20Types%20in%20Visual%20Basic%20\(Visual%20Basic\).md)   
 [Type List](../Topic/Type%20List%20\(Visual%20Basic\).md)   
 [Structure (Visual Basic)](assetId:///263ce115-ac36-4c05-8cb7-0e0eead5c6d0)   
 [Class (Visual Basic)](assetId:///0777c6e6-46bc-451b-ad70-57b49d4ef4f7)   
 [Value Types and Reference Types](../Topic/Value%20Types%20and%20Reference%20Types.md)