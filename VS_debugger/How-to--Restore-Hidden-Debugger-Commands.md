---
title: "How to: Restore Hidden Debugger Commands"
ms.custom: na
ms.date: 10/03/2016
ms.devlang: 
  - FSharp
  - VB
  - CSharp
  - C++
  - JScript
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
ms.assetid: 76ac9b77-f536-43b5-a9fc-984854b1c566
caps.latest.revision: 11
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
# How to: Restore Hidden Debugger Commands
When you set up Visual Studio, you are asked to choose a set of default IDE settings for your primary programming language. Default IDE settings for some languages may hide certain debugger commands.  
  
 If you want to use a debugger feature that is hidden by your default IDE settings, you can add the command back to the menu using the following procedure.  
  
### To restore hidden debugger commands  
  
1.  With a project open, on the **Tools** menu, click **Customize**.  
  
2.  In the **Customize** dialog box, click the **Commands** tab.  
  
3.  In the **Menu bar:** drop-down, select the **Debug** menu that you want to contain the restored command.  
  
4.  Click the **Add Command…** button.  
  
5.  In the **Add Command** box, select the command you want to add, and click **OK**.  
  
6.  Repeat the previous step to add another command.  
  
7.  Click **Close** when you have finished adding commands to the menu.  
  
    > [!WARNING]
    >  Some menu items only appear when the debugger is in specific modes, such as run mode or break mode. Therefore, an item you added may not be immediately visible when you complete these steps.  
  
## Restoring Commands Not Available from the Customize Dialog Box  
 Some commands, especially those found in hierarchical menus, cannot be restored from the **Customize** dialog box. To restore these commands, you must import a new collection of IDE settings.  
  
#### To import new IDE settings  
  
1.  On the **Tools** menu, click **Import and Export Settings**.  
  
2.  On the **Welcome to the Import and Export Settings Wizard** page, click **Import selected environment settings**, and then click **Next**.  
  
3.  On the **Save Current Settings** page, decide whether or not to save your existing settings, and then click **Next**.  
  
4.  On the **Choose a collection of settings to import** page, under the **Default Settings** folder, choose a collection of development settings that has the commands you want to use. If you do not know which collection to choose, try **General Development Settings** or **Visual C++ Development Settings**, which  provide the most debugger commands.  
  
5.  Click **Next**.  
  
6.  On the **Choose settings to import** page, under **Options**, make sure **Debugging** is selected. Clear the other check boxes, unless you want to import those settings as well.  
  
7.  Click **Finish**.  
  
8.  On the **Import Complete** page, review any errors associated with resetting your settings under **Details**.  
  
9. Click **Close**.  
  
## See Also  
 [Debugger Security](../VS_debugger/Debugger-Security.md)   
 [Debugger Basics](../VS_debugger/Debugger-Basics.md)