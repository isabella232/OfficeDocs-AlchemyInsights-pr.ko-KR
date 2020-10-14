---
title: EXO에서 메일을 사용 하 여 공용 폴더에 보내기
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451384"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="2413d-102">SendAs Mail Enabled 공용 폴더</span><span class="sxs-lookup"><span data-stu-id="2413d-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="2413d-103">다음 예에서는 사용자 Jason에 게 메일 사용이 가능한 공용 폴더 NewPF1에 대 한 "다른 사람 이름으로 보내기" 권한을 할당 합니다.</span><span class="sxs-lookup"><span data-stu-id="2413d-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="2413d-104">Add-RecipientPermission-Id ' NewPF1 '-트러스티 "Jason"-AccessRights ' SendAs '</span><span class="sxs-lookup"><span data-stu-id="2413d-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="2413d-105">자세한 구문 및 매개 변수 정보는 [메일 사용이 가능한 공용 폴더에 대해 "다른 사람 이름으로 보내기" 또는 "대신 보내기" 권한을](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="2413d-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>

