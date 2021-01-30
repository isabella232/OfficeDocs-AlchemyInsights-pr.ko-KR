---
title: 자격 증명 관련 문제
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052950"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="5862e-102">자격 증명 관련 문제</span><span class="sxs-lookup"><span data-stu-id="5862e-102">Issues with credentials</span></span>

<span data-ttu-id="5862e-103">Microsoft ID 플랫폼 및 [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 클라이언트 자격 증명 흐름에서는 OAuth 2.0 클라이언트 자격 증명에 대해 직접 프로그래밍하여 흐름을 부여하는 방법을 설명하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="5862e-104">**응용 프로그램의 암호 또는 인증서 자격 증명을 관리하는 방법**</span><span class="sxs-lookup"><span data-stu-id="5862e-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="5862e-105">Azure CLI에서 [az](https://docs.microsoft.com/cli/azure/ad/app/credential) 광고 앱 자격 증명을 사용하여 응용 프로그램의 암호 또는 인증서 자격 증명을 삭제, 목록 또는 다시 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="5862e-106">**사용자가 암호를 다시 설정하는 방법**</span><span class="sxs-lookup"><span data-stu-id="5862e-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="5862e-107">사용자가 암호를 [다시](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) 설정하려면 먼저 셀프 서비스 암호 재설정을 등록해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="5862e-108">사용자가 등록되면 이 문서의 지침에 따라 직장 또는 학교 암호를 다시 설정하여 암호를 다시 설정할 [수 있습니다.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)</span><span class="sxs-lookup"><span data-stu-id="5862e-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="5862e-109">**사용자가 암호를 변경하는 방법**</span><span class="sxs-lookup"><span data-stu-id="5862e-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="5862e-110">사용자는 이 문서의 단계에 따라 암호를 변경할 수 [있습니다. 암호를 변경하는 방법.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="5862e-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="5862e-111">또한 [2단계 인증을 위해 앱 암호를 관리할 수 있습니다.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="5862e-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="5862e-112">**사용자의 암호를 변경하거나 재설정할 때 오류가 발생했습니다.**</span><span class="sxs-lookup"><span data-stu-id="5862e-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="5862e-113">이 링크는 사용자가 암호를 다시 설정하려고 할 때 발생할 수 있는 일반적인 문제(일반적인 문제 및 해결 방법)에 [대한 정보를 제공합니다.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="5862e-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="5862e-114">**사용자의 암호를 다시 설정하는 데 문제가 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="5862e-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="5862e-115">암호를 재설정할 권한이 있는지 확인</span><span class="sxs-lookup"><span data-stu-id="5862e-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="5862e-116">*전역, 암호 및 사용자 관리자만 사용자 암호를 다시 설정할 수 있습니다.*</span><span class="sxs-lookup"><span data-stu-id="5862e-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="5862e-117">전역 관리자는 권한이 부여된 다른 관리자의 암호를 다시 설정할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="5862e-118">라이선스 요구 사항을 이해해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="5862e-119">조직에 라이선스가 하나 이상 할당되어 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="5862e-120">**클라우드 전용 사용자** - 모든 Office 365(O365) 유료 SKU 또는 Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="5862e-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="5862e-121">**클라우드 및/또는 프레미스** 사용자 - Azure AD Premium P1 또는 P2, EMS(Enterprise Mobility + Security) 또는 SPE(Secure Productive Enterprise)</span><span class="sxs-lookup"><span data-stu-id="5862e-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="5862e-122">라이선스 요구 사항에 대한 자세한 내용은 Azure AD 셀프 서비스 암호 재설정에 대한 [라이선스 요구 사항을 참조하세요.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="5862e-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="5862e-123">사용자의 암호를 다시 설정하기 위해 Azure AD에서 사용자를 찾아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="5862e-124">그런 다음 해당 사용자에 대한 개요 블레이드에서 "암호 재설정" 단추를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="5862e-125">**암호 재설정 단추가 회색으로 표시되어 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="5862e-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="5862e-126">이 사용자의 암호를 다시  설정할 수 있는 권한이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="5862e-127">*전역, 암호 및 사용자 관리자만 사용자 암호를 다시 설정할 수 있습니다.*</span><span class="sxs-lookup"><span data-stu-id="5862e-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="5862e-128">전역 관리자는 권한이 부여된 다른 관리자의 암호를 다시 설정할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="5862e-129">**암호 재설정 블레이드가 볼 수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="5862e-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="5862e-130">암호를 재설정할 수 있는 권한이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="5862e-131">*전역, 암호 및 사용자 관리자만 사용자 암호를 다시 설정할 수 있습니다.*</span><span class="sxs-lookup"><span data-stu-id="5862e-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="5862e-132">전역 관리자는 권한이 부여된 다른 관리자의 암호를 다시 설정할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="5862e-133">**암호 재설정 시에는 프레미스 통합 블레이드가 볼 수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="5862e-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="5862e-134">하이브리드 환경에서만 하이브리드 통합 블레이드가 나타납니다. 즉, 암호 쓰기 저장을 사용하여 On-premises 사용자의 암호를 조작합니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="5862e-135">다음 경우 이 블레이드가 표시되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="5862e-136">암호 쓰기 저장을 사용하고 있지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-136">You are not using password writeback</span></span>
  - <span data-ttu-id="5862e-137">암호 쓰기 저장의 설치/연결에 문제가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="5862e-138">Azure AD Connect의 설치/연결에 문제가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="5862e-139">암호 쓰기 저장 관련 문제에 대한 자세한 문제 해결 단계는 암호 쓰기 저장 [문제 해결을 참조하세요.](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="5862e-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="5862e-140">**사용자 암호를 다시 설정하는 방법을 모르는 경우**</span><span class="sxs-lookup"><span data-stu-id="5862e-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="5862e-141">Azure Portal에 적절한 관리자로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="5862e-142">사용자 및 그룹 **블레이드로** 이동하여 모든 **사용자를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="5862e-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="5862e-143">목록에서 사용자를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-143">Select a user from the list.</span></span>
4. <span data-ttu-id="5862e-144">선택한 사용자의 경우 개요를 선택한 다음 명령 표시줄에서 암호 **재설정을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="5862e-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="5862e-145">암호 다시 **설정 단추를** 선택하고 화면의 지침을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="5862e-146">Azure Portal을 통해 수행되는 **재설정만** 암호 쓰기 저장을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="5862e-147">**Office 365 관리 포털 또는 Office 365 모바일 응용 프로그램에서 해당 사용자의 암호를 다시 설정했지만 사용자가 여전히 로그인할 수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="5862e-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="5862e-148">암호 쓰기 저장은 이 포털에서 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5862e-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="5862e-149">Azure Portal에서 사용자의 암호를 다시 설정하십시오.</span><span class="sxs-lookup"><span data-stu-id="5862e-149">Reset the user's password again in the Azure portal.</span></span>
