---
title: Microsoft Edge에서 Azure 기능이 제대로 작동하지 않는 경우의 작업
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576483"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="a9402-102">Microsoft Edge에서 Azure 기능이 제대로 작동하지 않는 경우의 작업</span><span class="sxs-lookup"><span data-stu-id="a9402-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="a9402-103">Microsoft [Edge에는](https://go.microsoft.com/fwlink/?linkid=2140608) 보안 영역과 관련된 알려진 문제가 있으며 Azure 사용자가 Windows Admin Center에 로그인하는 방식에 영향을 줄 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9402-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="a9402-104">Microsoft Edge에서 Azure 기능을 사용하는 데 문제가 있는 경우 다음 단계를 시도해 하세요.</span><span class="sxs-lookup"><span data-stu-id="a9402-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="a9402-105">시작 **메뉴에서** 인터넷 옵션을 **검색하고** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="a9402-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="a9402-106">인터넷 속성 **대화 상자에서** 보안 **탭으로** 이동하십시오.</span><span class="sxs-lookup"><span data-stu-id="a9402-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="a9402-107">신뢰할 수 **있는 사이트 영역과** 사이트 **단추를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="a9402-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="a9402-108">신뢰할 수 **있는 사이트** 대화 상자에서 게이트웨이 URL도 추가하고 [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) 닫기를 **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="a9402-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="a9402-109">인터넷 속성 **대화 상자에서** 개인 정보 **탭으로** 이동하십시오.</span><span class="sxs-lookup"><span data-stu-id="a9402-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="a9402-110">팝업 차단 **섹션에서** 설정을 **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="a9402-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="a9402-111">대화 상자가 열리면 게이트웨이 URL도 추가하고 [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) 닫기를 **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="a9402-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
