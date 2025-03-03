---
description: "Loads the specified debug symbols in memory."
title: IDebugComPlusSymbolProvider::LoadSymbols
ms.date: 11/04/2016
ms.topic: reference
helpviewer_keywords:
- LoadSymbols
- IDebugComPlusSymbolProvider::LoadSymbols
author: maiak
ms.author: maiak
manager: jmartens
ms.technology: vs-ide-debug
dev_langs:
- CPP
- CSharp
---
# IDebugComPlusSymbolProvider::LoadSymbols

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Loads the specified debug symbols in memory.

## Syntax

### [C#](#tab/csharp)
```csharp
int LoadSymbols(
    uint   ulAppDomainID,
    Guid   guidModule,
    ulong  baseAddress,
    object pUnkMetadataImport,
    string bstrModuleName,
    string bstrSymSearchPath
);
```
### [C++](#tab/cpp)
```cpp
HRESULT LoadSymbols(
    ULONG32   ulAppDomainID,
    GUID      guidModule,
    ULONGLONG baseAddress,
    IUnknown* pUnkMetadataImport,
    BSTR      bstrModuleName,
    BSTR      bstrSymSearchPath
);
```
---

## Parameters
`ulAppDomainID`\
[in] Identifier of the application domain.

`guidModule`\
[in] Unique identifier of the mondule.

`baseAddress`\
[in] Base memory address.

`pUnkMetadataImport`\
[in] Object that contains the symbol metadata.

`bstrModuleName`\
[in] Name of the module.

`bstrSymSearchPath`\
[in] Path to search for the symbol file.

## Return Value
If successful, returns `S_OK`; otherwise, returns an error code.

## Example
The following example shows how to implement this method for a **CDebugSymbolProvider** object that exposes the [IDebugComPlusSymbolProvider](../../../extensibility/debugger/reference/idebugcomplussymbolprovider.md) interface.

```cpp
HRESULT CDebugSymbolProvider::LoadSymbols(
    ULONG32 ulAppDomainID,
    GUID guidModule,
    ULONGLONG baseOffset,
    IUnknown* _pMetadata,
    BSTR bstrModule,
    BSTR bstrSearchPath)
{
    return LoadSymbolsWithCorModule(ulAppDomainID, guidModule, baseOffset, _pMetadata, NULL, bstrModule, bstrSearchPath);
}
```

## See also
- [IDebugComPlusSymbolProvider](../../../extensibility/debugger/reference/idebugcomplussymbolprovider.md)
