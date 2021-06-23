---
title: SMTP 인증 활성화 및 문제 해결
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077657"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="85960-102">SMTP 인증 활성화 및 문제 해결</span><span class="sxs-lookup"><span data-stu-id="85960-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="85960-103">사서함에 대해 SMTP 인증을 사용하도록 설정하거나 Microsoft 365 장치 또는 응용 프로그램을 인증하여 전자 메일을 릴레이하려고 할 때 코드 5.7.57 또는 5.7.3 또는 5.7.139와 함께 "클라이언트가 인증되지 않음", "인증 실패" 또는 "SmtpClientAuthentication" 오류가 발생하는 경우 다음 세 가지 작업을 수행하여 문제를 해결하세요.</span><span class="sxs-lookup"><span data-stu-id="85960-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="85960-104">**보안 기본값 사용** 을 **아니요** 로 전환하여 [Azure 보안 기본값](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)을 비활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="85960-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="85960-105">a.</span><span class="sxs-lookup"><span data-stu-id="85960-105">a.</span></span> <span data-ttu-id="85960-106">Azure 포털에 보안 관리자, 조건부 액세스 관리자 또는 전역 관리자로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="85960-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="85960-107">b.</span><span class="sxs-lookup"><span data-stu-id="85960-107">b.</span></span> <span data-ttu-id="85960-108">Azure Active Directory>  **속성** 으로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="85960-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="85960-109">c.</span><span class="sxs-lookup"><span data-stu-id="85960-109">c.</span></span> <span data-ttu-id="85960-110">**보안 기본값 관리** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="85960-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="85960-111">d.</span><span class="sxs-lookup"><span data-stu-id="85960-111">d.</span></span> <span data-ttu-id="85960-112">**보안 기본값 사용** 을 **아니요** 로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="85960-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="85960-113">e.</span><span class="sxs-lookup"><span data-stu-id="85960-113">e.</span></span> <span data-ttu-id="85960-114">**저장** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="85960-114">Select **Save**.</span></span>

2. <span data-ttu-id="85960-115">라이선스가 있는 사서함에서 [클라이언트 SMTP 제출을 사용하도록 설정](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes)합니다.</span><span class="sxs-lookup"><span data-stu-id="85960-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="85960-116">a.</span><span class="sxs-lookup"><span data-stu-id="85960-116">a.</span></span> <span data-ttu-id="85960-117">Microsoft 365 관리 센터에서 **활성 사용자** 로 이동하여 사용자를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="85960-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="85960-118">b.</span><span class="sxs-lookup"><span data-stu-id="85960-118">b.</span></span> <span data-ttu-id="85960-119">메일 탭으로 이동하고 **이메일 앱** 에서 **이메일 앱 관리** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="85960-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="85960-120">d.</span><span class="sxs-lookup"><span data-stu-id="85960-120">d.</span></span> <span data-ttu-id="85960-121">**인증된 SMTP** 이(가) 선택(사용 설정)되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="85960-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="85960-122">e.</span><span class="sxs-lookup"><span data-stu-id="85960-122">e.</span></span> <span data-ttu-id="85960-123">**변경 사항 저장** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="85960-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="85960-124">라이선스가 부여된 사서함에서 [MFA(다단계 인증)를 비활성화](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa)합니다.</span><span class="sxs-lookup"><span data-stu-id="85960-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="85960-125">a.</span><span class="sxs-lookup"><span data-stu-id="85960-125">a.</span></span> <span data-ttu-id="85960-126">Microsoft 365 관리 센터로 이동하고 왼쪽 탐색 메뉴에서 **사용자** > **활성 사용자** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="85960-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="85960-127">b.</span><span class="sxs-lookup"><span data-stu-id="85960-127">b.</span></span> <span data-ttu-id="85960-128">**다단계 인증** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="85960-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="85960-129">c.</span><span class="sxs-lookup"><span data-stu-id="85960-129">c.</span></span> <span data-ttu-id="85960-130">사용자를 선택하고 **다단계 인증** 을 비활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="85960-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
