---
title: "Update a column when another table contains a reference to the row | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: ["cpp-windows"]
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: ["C++"]
helpviewer_keywords: ["rowsets, column updates"]
ms.assetid: abb5db69-055d-431f-b12d-ad2940a661ba
caps.latest.revision: 7
author: "mikeblome"
ms.author: "mblome"
manager: "ghogen"
---
# Updating a Column When Another Table Contains a Reference to the Row
Some providers can detect which columns in the row change, but many providers cannot. As a result, updating a column can result in an error when there is a reference to the row you are attempting to update. To solve this problem, create a separate accessor containing only the columns you want to change. Pass the number of that accessor to `SetData`.  
  
## See Also  
 [Using Accessors](../../data/oledb/using-accessors.md)