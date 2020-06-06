---
title: 사용 권한 상속
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bb5c440a-ca70-4dc6-b517-688e80551101
ms.openlocfilehash: 791085593433dcad9b800fdea8c7ea4a878604e7
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581057"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="d64f4-102">SharePoint에서 사용 권한 상속이 작동 하는 방식</span><span class="sxs-lookup"><span data-stu-id="d64f4-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="d64f4-103">기본적으로 SharePoint의 사용 권한은 계층 구조에서 위쪽 으로부터 상속 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d64f4-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="d64f4-104">따라서 파일은 해당 폴더에서 사용 권한을 상속 하며, 사이트에서 사용 권한을 상속 하며, 사이트 모음에서 사용 권한을 상속 합니다.</span><span class="sxs-lookup"><span data-stu-id="d64f4-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="d64f4-105">고유한 사용 권한을 제거 하 고 상속을 복원 하는 방법에 대 한 자세한 내용은 [목록 또는 라이브러리의 사용 권한 편집 및 관리](https://go.microsoft.com/fwlink/?linkid=869946)를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="d64f4-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

