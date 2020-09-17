---
title: autologon.microsoftazuread-sso.com:443 오류로 인해 Teams에 로그인할 수 없음
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 649124db135805d8101b43dbead63860d36853ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799966"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="47783-102">autologon.microsoftazuread-sso dot com:443 오류로 인해 Teams에 로그인할 수 없음</span><span class="sxs-lookup"><span data-stu-id="47783-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="47783-103">Seamless SSO가 O365 인증으로 활성화된 경우 URL "autologon.microsoftazuread-sso.com"을 인트라넷 사이트에 추가해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47783-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="47783-104">이전에 신뢰할 수 있는 사이트에 추가되었고 Seamless SSO가 사용 중인 경우 신뢰할 수 있는 사이트에서 제거해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="47783-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="47783-105">[Seamless SSO 문제 해결 검사 목록](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="47783-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="47783-106">인트라넷 사이트 목록에 URL을 추가하려면 다음 단계를 따르세요.</span><span class="sxs-lookup"><span data-stu-id="47783-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="47783-107">**시작** 버튼을 클릭하여 Internet Explorer를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="47783-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="47783-108">검색 상자에 Internet Explorer를 입력한 다음 결과 목록에서 **Internet Explorer**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="47783-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="47783-109">**도구**를 클릭한 다음 **인터넷 옵션**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="47783-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="47783-110">**보안** 탭을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="47783-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="47783-111">이제 **로컬 인트라넷 사이트**를 클릭한 다음 **사이트** 버튼과 **고급** 버튼을 차례로 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="47783-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="47783-112">웹 사이트 URL을 입력하고 **추가**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="47783-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="47783-113">작업을 마치면 **닫기**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="47783-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="47783-114">자세한 내용은 [O365용 Seamless SSO 배포 설명서](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start)(3 단계에서 인트라넷 사이트에 URL을 추가하는 정책 기반 프로세스 포함)를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="47783-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
