---
title: 사용자가 만든 전자 메일 서명 차단
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464875"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="92487-102">사용자가 만든 전자 메일 서명 차단</span><span class="sxs-lookup"><span data-stu-id="92487-102">Block user-made email signatures</span></span>

<span data-ttu-id="92487-103">다음 솔루션은 웹용 Outlook에서 만든 전자 메일 서명에만 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="92487-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="92487-104">Outlook 앱의 서명을 차단할 수 있는 것은 Outlook 앱의 프레미스 앱이 있는 Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="92487-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="92487-105">관리 센터에서 관리 센터 Exchange **를**  >  **선택 합니다.**</span><span class="sxs-lookup"><span data-stu-id="92487-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="92487-106">정책에 **대한**  >  **Outlook Web App 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="92487-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="92487-107">정책을 선택한 다음 연필 아이콘을 클릭하여 편집합니다.</span><span class="sxs-lookup"><span data-stu-id="92487-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="92487-108">기능 **추가 옵션**  >  **을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="92487-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="92487-109">사용자 **환경 아래에서** 전자 메일 서명 **확인란의** 선택을 취소한 다음 저장을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="92487-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="92487-110">**중요:** 이 확인란의 선택을 취소하기 전에 서명이 추가된 경우 사용자는 여전히 해당 확인란을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="92487-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="92487-111">제거를 요청합니다.</span><span class="sxs-lookup"><span data-stu-id="92487-111">Ask them to remove it.</span></span>
