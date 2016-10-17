---
title: "CLS Compliance Warning CLS01714"
ms.custom: na
ms.date: "10/13/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: na
ms.suite: na
ms.technology: 
  - "devlang-csharp"
ms.tgt_pltfrm: na
ms.topic: "article"
f1_keywords: 
  - "CLS01714"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "CLS01714"
ms.assetid: 8ba94d1e-ad27-4dd2-919a-19be75119e53
caps.latest.revision: 8
ms.author: "corob"
manager: "douge"
translation.priority.ht: 
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "ru-ru"
  - "zh-cn"
  - "zh-tw"
translation.priority.mt: 
  - "cs-cz"
  - "pl-pl"
  - "pt-br"
  - "tr-tr"
---
# CLS Compliance Warning CLS01714
Unmanaged pointer types are not CLS-compliant  
  
 A CLS-compliant delegate signature cannot contain an unmanaged pointer type.  
  
 For more information Common Language Subset (CLS) compliance checking, see [CLS Compliant Assemblies](assetId:///3320b57e-ea55-4697-a17d-f509a36a3c93).  
  
 The following sample generates CLS01714:  
  
```  
// CLS01714.cpp  
// compile with: /clr /LD  
// CLS01714 expected  
using namespace System;  
using namespace System::Reflection;  
[assembly:CLSCompliant (true)];  
[assembly:AssemblyKeyFile("clscompliance.snk")];  
public delegate void MyDelegate1(int* Parameter);   // CLS01714  
```