---
title: ObjectFrame.DisplayWhen property (Access)
keywords: vbaac10.chm11580
f1_keywords:
- vbaac10.chm11580
ms.prod: access
api_name:
- Access.ObjectFrame.DisplayWhen
ms.assetid: 37e03fc6-aee9-b6cf-eafb-7af111b5b9e3
ms.date: 02/21/2019
ms.localizationpriority: medium
---


# ObjectFrame.DisplayWhen property (Access)

Use the **DisplayWhen** property to specify which of a form's controls you want displayed on screen and in print. Read/write **Byte**.


## Syntax

_expression_.**DisplayWhen**

_expression_ A variable that represents an **[ObjectFrame](Access.ObjectFrame.md)** object.


## Remarks

The **DisplayWhen** property applies only to the following form sections: detail, form header, and form footer. It also applies to all controls (except page breaks) on a form.

The **DisplayWhen** property uses the following settings.

|Setting|Visual Basic|Description|
|:-----|:-----|:-----|
|Always|0|(Default) The object appears in Form view and when printed.|
|Print Only|1|The object is hidden in Form view but appears when printed.|
|Screen Only|2|The object appears in Form view but not when printed.|

For controls, you can set the default for this property by using the default control style or the **[DefaultControl](access.form.defaultcontrol.md)** property in Visual Basic.

In many cases, certain controls are useful only in Form view. To prevent Microsoft Access from printing these controls, you can set their **DisplayWhen** property to Screen Only. For example, you might have a command button or instructions on a form that you don't want printed, or you might have form header and form footer sections that you don't want displayed on screen but that you do want printed. In this case, you should set the **DisplayWhen** property to Print Only.

For reports, use the **Format** and **Retreat** events to specify an event procedure or macro that sets the **Visible** property of controls that you don't want printed. You can also cancel the **Format** or **Print** event for a report section to prevent the section from being printed.


[!include[Support and feedback](~/includes/feedback-boilerplate.md)]