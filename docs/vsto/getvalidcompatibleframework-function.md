---
title: "GetValidCompatibleFramework function"
description: Learn how the GetValidCompatibleFramework API supports the Office infrastructure and isn't intended to be used directly from your code.
ms.date: "02/02/2017"
ms.topic: "reference"
dev_langs:
  - "VB"
  - "CSharp"
author: John-Hart
ms.author: johnhart
manager: jmartens
ms.technology: office-development
---
# GetValidCompatibleFramework function

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
  This API supports the Office infrastructure and isn't intended to be used directly from your code.

## Syntax

```csharp
HRESULT WINAPI GetValidCompatibleFramework(
    LPCWSTR lpwszCompatibleFrameworksXML,
    BSTR* pbstrValidFrameworkTag
);
```

### Parameters

|Parameter|Description|
|---------------|-----------------|
|*lpwszCompatibleFrameworksXML*|Don't use.|
|*pbstrValidFrameworkTag*|Don't use.|

## Return value
 If the function succeeds, it returns **S_OK**. If the function fails, it returns an error code.
