---
title: "Unmanaged API reference (Office development in Visual Studio)"
description: The unmanaged API reference is used to help load-managed VSTO Add-ins. You can also create your own VSTO Add-in loader component by implementing this interface.
titleSuffix: ""
ms.date: "08/14/2019"
ms.topic: "reference"
dev_langs:
  - "VB"
  - "CSharp"
helpviewer_keywords:
  - "Office development in Visual Studio, reference"
  - "Office development in Visual Studio, unmanaged API reference"
author: John-Hart
ms.author: johnhart
manager: jmartens
ms.technology: office-development
---
# Unmanaged API reference (Office development in Visual Studio)

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]

Starting with the 2007 Microsoft Office system, Office applications use the [IManagedAddin interface](../vsto/imanagedaddin-interface.md) interface to call into a VSTO Add-in loader component that is included with the  Visual Studio Tools for Office runtime . This component is used to help load-managed VSTO Add-ins. You can create your own VSTO Add-in loader component by implementing this interface.

[!include[Add-ins note](includes/addinsnote.md)]

## In this section

[IManagedAddin interface](../vsto/imanagedaddin-interface.md)

A COM interface that you can implement to load and unload managed VSTO Add-ins in Office applications.
