---
title: 如何提供文件操作进度对话框 - C# 编程指南
description: 了解如何使用 CopyFile (String, String, UIOption) 方法为文件操作提供进度对话框。
ms.date: 07/20/2015
helpviewer_keywords:
- progress dialog [C#]
ms.assetid: 01b71fe7-8178-4dc8-aeb1-12053be7b51c
ms.openlocfilehash: 2ea18d924b47fc10412d37479f1b09f7eef7ad3b
ms.sourcegitcommit: 6f58a5f75ceeb936f8ee5b786e9adb81a9a3bee9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "87301965"
---
# <a name="how-to-provide-a-progress-dialog-box-for-file-operations-c-programming-guide"></a>如何提供文件操作进度对话框（C# 编程指南）
如果在 <xref:Microsoft.VisualBasic?displayProperty=nameWithType> 命名空间中使用 <xref:Microsoft.VisualBasic.FileIO.FileSystem.CopyFile%28System.String%2CSystem.String%2CMicrosoft.VisualBasic.FileIO.UIOption%29> 方法，可以在 Windows 中提供显示文件操作进度的标准对话框。  
  
[!INCLUDE[note_settings_general](~/includes/note-settings-general-md.md)]  
  
### <a name="to-add-a-reference-in-visual-studio"></a>在 Visual Studio 中添加引用  
  
1. 在菜单栏上，依次选择“项目”、“添加引用”。  
  
     此时将显示“引用管理器”对话框。  
  
2. 在“程序集”区域，选择“Framework”（如果尚未选择它）。  
  
3. 在名称列表中，选择“Microsoft.VisualBasic”复选框，然后再选择“确定”按钮以关闭对话框。  
  
## <a name="example"></a>示例  
 以下代码将 `sourcePath` 指定的目录复制到 `destinationPath` 指定的目录。 此代码还提供了标准的对话框，其中显示在操作完成前估计的剩余时间量。  
  
 [!code-csharp[csFilesandFolders#11](~/samples/snippets/csharp/VS_Snippets_VBCSharp/csFilesAndFolders/CS/FileIteration.cs#11)]  
  
## <a name="see-also"></a>请参阅

- [文件系统和注册表（C# 编程指南）](./index.md)
