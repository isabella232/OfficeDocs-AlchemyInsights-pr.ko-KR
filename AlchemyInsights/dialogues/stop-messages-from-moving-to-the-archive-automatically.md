---
title: 메시지가 자동으로 보관함으로 이동하지 못하게 중지
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50522420"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="15c55-102">메시지가 자동으로 보관함으로 이동하지 못하게 중지</span><span class="sxs-lookup"><span data-stu-id="15c55-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="15c55-103">보존 정책을 사용하는 경우 해당 정책의 보존 기간을 변경하여 메시지가 자동으로 보관되지 못하게 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="15c55-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="15c55-104">방법은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="15c55-104">Here's how:</span></span>

1. <span data-ttu-id="15c55-105">Exchange 관리 [센터에서](https://go.microsoft.com/fwlink/?linkid=2059104)준수 **관리 보존**  >  **태그 를 선택 합니다.**</span><span class="sxs-lookup"><span data-stu-id="15c55-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="15c55-106">보관함으로 이동 보존 태그를 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="15c55-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="15c55-107">보존 태그에서 보존 정책에 의해 항목이  자동으로 보관되는 것을 중지하기 위해 보존 기간(보관 기간)을 사용 안 함으로 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="15c55-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="15c55-108">이렇게 하면 이 보존 태그가 적용된 모든 사서함의 보관 설정이 변경됩니다.</span><span class="sxs-lookup"><span data-stu-id="15c55-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
