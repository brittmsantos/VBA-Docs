---
title: DoCmd.Maximize method (Access)
keywords: vbaac10.chm4156
f1_keywords:
- vbaac10.chm4156
ms.prod: access
api_name:
- Access.DoCmd.Maximize
ms.assetid: 6b1103f5-07b8-fbcf-ff7e-ccbfd6945768
ms.date: 03/07/2019
ms.localizationpriority: medium
---


# DoCmd.Maximize method (Access)

The **Maximize** method carries out the Maximize action in Visual Basic.


## Syntax

_expression_.**Maximize**

_expression_ A variable that represents a **[DoCmd](Access.DoCmd.md)** object.


## Remarks

Use the **Maximize** method to enlarge the active window so that it fills the Microsoft Access window. This action will allow you to see as much of the object in the active window as possible.

Use the **Restore** method to restore a maximized window to its previous size.

You may need to use the **SelectObject** method if the window that you want to maximize isn't the active window.

When you maximize a window in Access, all other windows are also maximized when you open them or switch to them. However, pop-up forms aren't maximized. If you want a form to maintain its size when other windows are maximized, set its **PopUp** property to **True**.

This method cannot be applied to module windows in the Visual Basic Editor (VBE). For information about how to affect module windows, see the **[WindowState](excel.window.windowstate.md)** property topic.



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]
