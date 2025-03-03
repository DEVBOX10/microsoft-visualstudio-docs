---
description: "Retrieves the number of value strings to display for the specified property or field."
title: IEEVisualizerService::GetValueDisplayStringCount
ms.date: 11/04/2016
ms.topic: reference
helpviewer_keywords:
- IEEVisualizerService::GetValueDisplayStringCount
- GetValueDisplayStringCount
author: maiak
ms.author: maiak
manager: jmartens
ms.technology: vs-ide-debug
dev_langs:
- CPP
- CSharp
---
# IEEVisualizerService::GetValueDisplayStringCount

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Retrieves the number of value strings to display for the specified property or field.

## Syntax

### [C#](#tab/csharp)
```csharp
int GetValueDisplayStringCount (
   uint        displayKind,
   IDebugField propertyOrField,
   out ulong   pcelt
);
```
### [C++](#tab/cpp)
```cpp
HRESULT GetValueDisplayStringCount (
   DWORD         displayKind,
   IDebugField * propertyOrField,
   ULONG *       pcelt
);
```
---

## Parameters
`displayKind`\
[in] Value from the [DisplayKind](../../../extensibility/debugger/reference/displaykind.md) enumeration.

`propertyOrField`\
[in] An [IDebugField](../../../extensibility/debugger/reference/idebugfield.md) interface that represents a property or field.

`pcelt`\
[out] Returns the number of value strings to display.

## Return Value
 If successful, returns `S_OK`; otherwise, returns an error code.

## See also
- [IEEVisualizerService](../../../extensibility/debugger/reference/ieevisualizerservice.md)
