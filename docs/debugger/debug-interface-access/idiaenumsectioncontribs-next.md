---
description: "Retrieves a specified number of section contributions in the enumeration sequence."
title: "IDiaEnumSectionContribs::Next"
ms.date: "11/04/2016"
ms.topic: "reference"
dev_langs:
  - "C++"
helpviewer_keywords:
  - "IDiaEnumSectionContribs::Next method"
author: "mikejo5000"
ms.author: "mikejo"
manager: jmartens
ms.technology: vs-ide-debug
---
# IDiaEnumSectionContribs::Next

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Retrieves a specified number of section contributions in the enumeration sequence.

## Syntax

```C++
HRESULT Next( 
   ULONG                celt,
   IDiaSectionContrib** rgelt,
   ULONG*               pceltFetched
);
```

#### Parameters
 celt

[in] The number of section contributions in the enumerator to be retrieved.

 rgelt

[out] An array that is to be filled with the [IDiaSectionContrib](../../debugger/debug-interface-access/idiasectioncontrib.md) objects that represent the desired section contributions.

 pceltFetched

[out] Returns the number of section contributions in the enumerator fetched.

## Return Value
 If successful, returns `S_OK`. Returns `S_FALSE` if there are no more section contributions. Otherwise, returns an error code.

## See also
- [IDiaEnumSectionContribs](../../debugger/debug-interface-access/idiaenumsectioncontribs.md)
- [IDiaSectionContrib](../../debugger/debug-interface-access/idiasectioncontrib.md)
