---
title: CorSymSearchPolicyAttributes 枚举
ms.date: 03/30/2017
api_name:
- CorSymSearchPolicyAttributes
api_location:
- mscoree.dll
api_type:
- COM
f1_keywords:
- CorSymSearchPolicyAttributes
helpviewer_keywords:
- CorSymSearchPolicyAttributes enumeration [.NET Framework debugging]
ms.assetid: 03abde84-930a-49d3-bac3-23abb34a0184
topic_type:
- apiref
ms.openlocfilehash: 8af71314cf8a24c710d3b8980c082daaf9186715
ms.sourcegitcommit: da21fc5a8cce1e028575acf31974681a1bc5aeed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2020
ms.locfileid: "84501867"
---
# <a name="corsymsearchpolicyattributes-enumeration"></a>CorSymSearchPolicyAttributes 枚举
指定在搜索符号读取器时要使用的策略。 [ISymUnmanagedBinder2：： GetReaderForFile2](isymunmanagedbinder2-getreaderforfile2-method.md)和[ISymUnmanagedBinder3：： GetReaderFromCallback](isymunmanagedbinder3-getreaderfromcallback-method.md)方法使用这些常量。  
  
> [!IMPORTANT]
> 打开不受信任的源中的程序数据库（PDB）文件会带来安全风险。  
  
## <a name="syntax"></a>语法  
  
```cpp  
typedef enum CorSymSearchPolicyAttributes  
{  
    AllowRegistryAccess      = 0x1,
    AllowSymbolServerAccess  = 0x2,  
    AllowOriginalPathAccess  = 0x4,     //
    AllowReferencePathAccess = 0x8  
} CorSymSearchPolicyAttributes;  
```  
  
## <a name="members"></a>成员  
  
|成员|描述|  
|------------|-----------------|  
|`AllowRegistryAccess`|在注册表中查询符号搜索路径。|  
|`AllowSymbolServerAccess`|访问符号服务器。|  
|`AllowOriginalPathAccess`|搜索在调试目录中指定的路径。|  
|`AllowReferencePathAccess`|搜索 .exe 文件所在位置的 PDB。|  
  
## <a name="requirements"></a>要求  
 **标头：** CorSym，CorSym  
  
## <a name="see-also"></a>另请参阅

- [诊断符号存储区枚举](diagnostics-symbol-store-enumerations.md)
