---
title: SSPR 문제 해결
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428834"
---
# <a name="troubleshoot-sspr"></a><span data-ttu-id="99b3d-102">SSPR 문제 해결</span><span class="sxs-lookup"><span data-stu-id="99b3d-102">Troubleshoot SSPR</span></span>

<span data-ttu-id="99b3d-103">**암호 재설정을 구성하는 데 문제가 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="99b3d-103">**I'm having trouble configuring password reset**</span></span>

- <span data-ttu-id="99b3d-104">셀프 서비스 암호 재설정을 사용하도록 설정하는 방법을 찾고 있는 경우 [자습서 SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)사용 을 참조하여 조직에 대한 암호 재설정을 구성합니다.</span><span class="sxs-lookup"><span data-stu-id="99b3d-104">If you are administrator and looking for how to enable self-service password reset, see [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization.</span></span> <span data-ttu-id="99b3d-105">라이선스 요구 사항을 [검토할 수도 있습니다.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="99b3d-105">You may also want to review the [licensing requirements](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span> <span data-ttu-id="99b3d-106">조직에 라이선스가 하나 이상 할당되어 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="99b3d-106">You must have at least one license assigned in your organization.</span></span>
    - <span data-ttu-id="99b3d-107">**클라우드 전용 사용자** - Office 365(O365) 유료 SKU 또는 Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="99b3d-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="99b3d-108">**클라우드 및/또는** 사내 사용자 - Azure AD Premium P1 또는 P2, EMS(Enterprise Mobility + Security) 또는 SPE(Secure Productive Enterprise)</span><span class="sxs-lookup"><span data-stu-id="99b3d-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
- <span data-ttu-id="99b3d-109">셀프 서비스 암호 재설정에 대한 자세한 질문은 [FAQ를 검토하세요.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="99b3d-109">For additional questions about self-service password reset, review [our FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="99b3d-110">**오류 메시지가 표시**</span><span class="sxs-lookup"><span data-stu-id="99b3d-110">**I'm getting an error message**</span></span>

<span data-ttu-id="99b3d-111">이 문서를 검토하여 일반적인 오류 및 해당 해결 방법 찾기: [셀프 서비스](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support) 암호 재설정 문제 해결</span><span class="sxs-lookup"><span data-stu-id="99b3d-111">Review this article to find common errors and their solutions: [Troubleshoot self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="99b3d-112">**암호 재설정 정책에 문제가 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="99b3d-112">**I'm having a problem with my password reset policy**</span></span>

- <span data-ttu-id="99b3d-113">암호 재설정 정책이 예상대로 행동하지 않는 경우 또는 암호 재설정 정책에 대한 질문이 있는 경우 이 문서를 검토하세요. [Azure Active Directory의](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)암호 정책 및 제한 사항.</span><span class="sxs-lookup"><span data-stu-id="99b3d-113">If your password reset policy is not behaving as expected, or if you have questions about password reset policies, review this article: [Password policies and restrictions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="99b3d-114">암호 재설정 정책은 관리자에게 적용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="99b3d-114">Password reset policies do not apply to administrators.</span></span> <span data-ttu-id="99b3d-115">Microsoft는 Azure 관리자 역할에 대해 강력한 기본 2 게이트 암호 재설정 정책을 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="99b3d-115">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role.</span></span> <span data-ttu-id="99b3d-116">관리자가 아닌 사용자와 테스트하는지 확인</span><span class="sxs-lookup"><span data-stu-id="99b3d-116">Make sure that you are testing with a user who is not an administrator.</span></span> <span data-ttu-id="99b3d-117">관리자 재설정 정책에 대한 자세한 내용은 이 문서를 [참조하세요. 관리자](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)재설정 정책 차이점 .</span><span class="sxs-lookup"><span data-stu-id="99b3d-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span></span>

<span data-ttu-id="99b3d-118">**사용자가 암호 재설정을 위한 추가 보안 정보를 등록하지 못하게 하려는 경우**</span><span class="sxs-lookup"><span data-stu-id="99b3d-118">**I don't want my users to register additional security info for password reset**</span></span>

<span data-ttu-id="99b3d-119">API, PowerShell 또는 Azure AD Connect를 사용하여 사용자에 대한 데이터(전자 메일 및 전화 특성)를 미리 채우면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="99b3d-119">You can pre-populate data (email and phone attributes) for your users using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="99b3d-120">읽기 방법을 알아보는 방법:</span><span class="sxs-lookup"><span data-stu-id="99b3d-120">To learn how read:</span></span>

- [<span data-ttu-id="99b3d-121">사용자가 등록할 필요 없이 암호 재설정 배포</span><span class="sxs-lookup"><span data-stu-id="99b3d-121">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [<span data-ttu-id="99b3d-122">암호 재설정에 사용되는 데이터</span><span class="sxs-lookup"><span data-stu-id="99b3d-122">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="99b3d-123">**사용자가 암호 재설정을 위한 추가 보안 정보를 등록할 수 있도록 하려는 경우**</span><span class="sxs-lookup"><span data-stu-id="99b3d-123">**I want my users to register their additional security info for password reset**</span></span>

1. <span data-ttu-id="99b3d-124">사용자가 셀프 서비스 암호 재설정에 대한 보안 정보를 등록할 수 있도록 에서 로 [aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)</span><span class="sxs-lookup"><span data-stu-id="99b3d-124">Have your users register their security info for self service password reset by directing them to [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span></span>
1. <span data-ttu-id="99b3d-125">사용자 또는 관리자가 사용자에 대해 데이터를 채우고 나면 사용자가 [](https://passwordreset.microsoftonline.com/) 암호를 다시 aka.ms/sspr 권한을 부여할 수 있도록 사용자에게 지시합니다.</span><span class="sxs-lookup"><span data-stu-id="99b3d-125">After data is populated for the user (by the user or by the admin), direct your user to [aka.ms/sspr](https://passwordreset.microsoftonline.com/) so your users can be empowered to reset their own passwords.</span></span>
1. <span data-ttu-id="99b3d-126">사용자가 여전히 문제가 발생하는 경우 페더링 또는 암호 해시 동기화된 사용자일 가능성이 **높습니다.** </span><span class="sxs-lookup"><span data-stu-id="99b3d-126">If users are still experiencing problems they are most likely **federated** or **password hash synched** users.</span></span> <span data-ttu-id="99b3d-127">즉, 암호 쓰기 저장 서비스에 문제가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="99b3d-127">This means there is likely a problem with the Password Writeback service.</span></span>