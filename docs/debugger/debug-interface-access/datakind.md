---
description: "Indicates the particular scope of a data value."
title: "DataKind"
ms.date: "11/04/2016"
ms.topic: "reference"
dev_langs:
  - "C++"
helpviewer_keywords:
  - "DataKind enumeration"
author: "mikejo5000"
ms.author: "mikejo"
manager: mijacobs
ms.subservice: debug-diagnostics
---
# DataKind

Indicates the particular scope of a data value.

## Syntax

```C++
enum DataKind {
    DataIsUnknown,
    DataIsLocal,
    DataIsStaticLocal,
    DataIsParam,
    DataIsObjectPtr,
    DataIsFileStatic,
    DataIsGlobal,
    DataIsMember,
    DataIsStaticMember,
    DataIsConstant
};
```

## Elements

| Element    | Description                                      |
| ------------------ | ---------------------------------------- |
| DataIsUnknown      | Data symbol cannot be determined.        |
| DataIsLocal        | Data item is a local variable.           |
| DataIsStaticLocal  | Data item is a static local variable.    |
| DataIsParam        | Data item is a formal parameter.         |
| DataIsObjectPtr    | Data item is an object pointer (`this`). |
| DataIsFileStatic   | Data item is a file-scoped variable.     |
| DataIsGlobal       | Data item is a global variable.          |
| DataIsMember       | Data item is an object member variable.  |
| DataIsStaticMember | Data item is a class static variable.    |
| DataIsConstant     | Data item is a constant value.           |

## Remarks
The values in this enumeration are returned by the [IDiaSymbol::get_dataKind](../../debugger/debug-interface-access/idiasymbol-get-datakind.md) method.

## Requirements
Header: cvconst.h

## See also
- [Enumerations and Structures](../../debugger/debug-interface-access/enumerations-and-structures.md)
- [IDiaSymbol::get_dataKind](../../debugger/debug-interface-access/idiasymbol-get-datakind.md)
