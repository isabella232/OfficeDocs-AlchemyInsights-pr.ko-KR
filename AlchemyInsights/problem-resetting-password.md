---
title: 암호 재설정 문제
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50585653"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="586ae-102">암호 재설정 문제</span><span class="sxs-lookup"><span data-stu-id="586ae-102">Problems resetting password</span></span>

<span data-ttu-id="586ae-103">다음은 암호를 재설정할 때 직면할 수 있는 몇 가지 문제와 가능한 해결 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="586ae-104">**다른 범주에서 다루지 않는 암호 재설정에 문제가 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="586ae-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="586ae-105">암호를 재설정할 수 있는 권한이 부여된지 확인</span><span class="sxs-lookup"><span data-stu-id="586ae-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="586ae-106">전역, 암호 및 사용자 관리자만 사용자 암호를 재설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="586ae-107">전역 관리자는 권한이 부여된 다른 관리자의 암호를 다시 설정할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="586ae-108">라이선스 요구 사항을 이해해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="586ae-109">조직에 라이선스가 하나 이상 할당되어 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="586ae-110">클라우드 전용 사용자 - Office 365(O365) 유료 SKU 또는 Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="586ae-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="586ae-111">클라우드 및/또는 사내 사용자 - Azure AD Premium P1 또는 P2, EMS(Enterprise Mobility + Security) 또는 SPE(Secure Productive Enterprise)</span><span class="sxs-lookup"><span data-stu-id="586ae-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="586ae-112">라이선스 요구 사항에 대한 자세한 내용은 Azure AD 셀프 서비스 암호 재설정에 대한 라이선스 요구 [사항을 참조하세요.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="586ae-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="586ae-113">**설정한 암호 재설정 정책 테스트에 문제가 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="586ae-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="586ae-114">최근에 적용된 정책은 모든 데이터 센터 및 끝점에서 복제하는 데 몇 분 정도 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="586ae-115">데이터 센터와의 물리적 거리는 변경 내용이 적용되는 방식에도 영향을 미치게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="586ae-116">관리자가 아닌 최종 사용자와 테스트하고 소수의 사용자로 파일럿을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="586ae-117">Azure Portal에 구성된 정책은 관리자가 아닌 최종 사용자에게만 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="586ae-118">Microsoft는 모든 Azure 관리자 역할에 대해 강력한 기본 2 게이트 암호 재설정 정책을 적용합니다(예: 전역 관리자, 헬프데스크 관리자, 암호 관리자 등).</span><span class="sxs-lookup"><span data-stu-id="586ae-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="586ae-119">관리자의 정책에 [대해 자세히 알아보시고 을(를) 자세히 알아보아야 합니다.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="586ae-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="586ae-120">**암호 재설정을 배포하고 싶지만 사용자가 추가 보안 정보를 등록할 수 있도록 하고 싶지 않습니다.**</span><span class="sxs-lookup"><span data-stu-id="586ae-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="586ae-121">사용자에 대한 데이터를 미리 채우면 사용자가 할 일도 없습니다!</span><span class="sxs-lookup"><span data-stu-id="586ae-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="586ae-122">- 관리자는 조직에 암호 재설정을 롤아웃하기 전에 사용자의 전화 및 전자 메일 속성을 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="586ae-123">API, PowerShell 또는 Azure AD Connect를 사용하여 이 작업을 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="586ae-124">자세한 내용은 다음을 참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="586ae-124">More information here:</span></span>
- [<span data-ttu-id="586ae-125">사용자가 등록할 필요 없이 암호 재설정 배포</span><span class="sxs-lookup"><span data-stu-id="586ae-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="586ae-126">암호 재설정에 사용되는 데이터</span><span class="sxs-lookup"><span data-stu-id="586ae-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="586ae-127">**암호 재설정 단추가 회색으로 표시되어 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="586ae-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="586ae-128">이 사용자의 암호를 다시 설정할 수 있는 권한이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="586ae-129">전역, 암호 및 사용자 관리자만 사용자 암호를 재설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="586ae-130">전역 관리자는 권한이 부여된 다른 관리자의 암호를 다시 설정할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="586ae-131">**암호 재설정 블레이드가 표시되지 않습니다.**</span><span class="sxs-lookup"><span data-stu-id="586ae-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="586ae-132">암호를 재설정할 수 있는 권한이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="586ae-133">전역, 암호 및 사용자 관리자만 사용자 암호를 재설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="586ae-134">전역 관리자는 권한이 부여된 다른 관리자의 암호를 다시 설정할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="586ae-135">**암호 재설정 시에는 프레미스 통합 블레이드가 볼 수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="586ae-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="586ae-136">사내 통합 블레이드는 하이브리드 환경에서만 나타납니다. 즉, 암호 쓰기 저장을 사용하여 On-premises 사용자의 암호를 조작할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="586ae-137">다음 경우 이 블레이드가 표시되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="586ae-138">암호 쓰기 저장을 사용하고 있지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-138">You are not using password writeback</span></span>
    - <span data-ttu-id="586ae-139">암호 쓰기 저장 설치/연결에 문제가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="586ae-140">Azure AD Connect의 설치/연결에 문제가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="586ae-141">암호 쓰기 저장 관련 문제에 대한 자세한 문제 해결 단계는 암호 쓰기 저장 문제 [해결 섹션을 참조하세요.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="586ae-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="586ae-142">**사용자 암호를 다시 설정하는 방법을 모르는 경우**</span><span class="sxs-lookup"><span data-stu-id="586ae-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="586ae-143">Azure Portal에 적절한 관리자로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="586ae-144">사용자 및 그룹 블레이드로 이동하여 모든 사용자를 **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="586ae-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="586ae-145">목록에서 사용자를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-145">Select a user from the list.</span></span>
1. <span data-ttu-id="586ae-146">선택한 사용자에 대해 개요를 선택한 다음 명령 표시줄에서 암호 다시 설정을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="586ae-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="586ae-147">화면의 지시를 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="586ae-148">Azure Portal에서 암호 쓰기 저장을 지원하는 데만 수행되는 재설정입니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="586ae-149">**Office 365 관리 포털 또는 Office 365 모바일 응용 프로그램에서 사용자의 암호를 다시 설정했지만 사용자가 여전히 로그인할 수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="586ae-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="586ae-150">암호 쓰기 저장은 이 포털에서 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="586ae-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="586ae-151">Azure Portal에서 사용자 암호를 다시 portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="586ae-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

