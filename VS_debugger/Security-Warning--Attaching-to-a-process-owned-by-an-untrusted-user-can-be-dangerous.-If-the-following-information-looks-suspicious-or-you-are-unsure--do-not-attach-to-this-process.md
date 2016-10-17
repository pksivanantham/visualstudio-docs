---
title: "Security Warning: Attaching to a process owned by an untrusted user can be dangerous. If the following information looks suspicious or you are unsure, do not attach to this process"
ms.custom: na
ms.date: 10/03/2016
ms.devlang: 
  - FSharp
  - VB
  - CSharp
  - C++
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - vs-ide-debug
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 52246c1e-a371-40a0-b756-a435cc51876f
caps.latest.revision: 14
manager: ghogen
translation.priority.ht: 
  - cs-cz
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - pl-pl
  - pt-br
  - ru-ru
  - tr-tr
  - zh-cn
  - zh-tw
---
# Security Warning: Attaching to a process owned by an untrusted user can be dangerous. If the following information looks suspicious or you are unsure, do not attach to this process
This warning dialog box appears when you attach to a process that contains partially trusted code or is owned by an untrusted user immediately before the attach occurs. An untrusted process that contains malicious code has the potential to damage the computer doing the debugging. If you have reason to distrust the process, then you should click **Cancel** to prevent debugging.  
  
 To suppress this warning when debugging a legitimate scenario, close Visual Studio, and set the value of this registry key to 1: `HKEY_CURRENT_USER\Software\Microsoft\VisualStudio\<version>\Debugger\DisableAttachSecurityWarning`, and then restart Visual Studio. After you finish debugging the scenario, reset the value to 0, and restart Visual Studio.  
  
 "Trusted users" include yourself, plus a set of standard users who are typically defined on computers that have the .NET Framework installed, such as `aspnet`, `localsystem`, `networkservice`, and `localservice`.  
  
## UIElement List  
 Name  
 Name of the assembly requested to debug  
  
 User  
 Current user  
  
 Attach  
 Press to continue to debug by attaching  
  
 Don't Attach  
 Do not attach to the process  
  
## See Also  
 [Attach to Running Processes](../VS_debugger/Attach-to-Running-Processes-with-the-Visual-Studio-Debugger.md)   
 [Debugger Security](../VS_debugger/Debugger-Security.md)