---
title: 설치 DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808713"
---
# <a name="setup-dkim"></a><span data-ttu-id="cf020-102">설치 DKIM</span><span class="sxs-lookup"><span data-stu-id="cf020-102">Setup DKIM</span></span>

<span data-ttu-id="cf020-103">Microsoft 365에서 사용자 지정 도메인에 대 한 DKIM을 구성 하기 위한 전체 지침은 [여기](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)에 나와 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf020-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="cf020-104">**각** 사용자 지정 도메인에 대해 도메인의 DNS 호스팅 서비스 (대개 도메인 등록자)에서 **두 개의** dkim CNAME 레코드를 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf020-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="cf020-105">예를 들어 contoso.com 및 fourthcoffee.com에는 4 개의 DKIM CNAME 레코드 (contoso.com의 경우 2, fourthcoffee.com의 경우 2)가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf020-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="cf020-106">**각** 사용자 지정 도메인에 대 한 DKIM CNAME 레코드에는 다음과 같은 형식이 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="cf020-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="cf020-107">**호스트 이름**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="cf020-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="cf020-108">**주소 또는 값을 가리킵니다**. `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="cf020-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="cf020-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="cf020-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="cf020-110">**호스트 이름**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="cf020-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="cf020-111">**주소 또는 값을 가리킵니다**. `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="cf020-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="cf020-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="cf020-112">**TTL**: 3600</span></span>

   <span data-ttu-id="cf020-113">\<DomainGUID\> 은 `.mail.protection.outlook.com` 사용자 지정 도메인 (예: `contoso-com` contoso.com 도메인)에 대해 사용자 지정한 MX 레코드의 왼쪽에 있는 텍스트입니다.</span><span class="sxs-lookup"><span data-stu-id="cf020-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="cf020-114">\<InitialDomain\> 은 Microsoft 365에 등록할 때 사용한 도메인 (예: contoso.onmicrosoft.com)입니다.</span><span class="sxs-lookup"><span data-stu-id="cf020-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="cf020-115">사용자 지정 도메인에 대 한 CNAME 레코드를 만든 후에는 다음 지침을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="cf020-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="cf020-116">a.</span><span class="sxs-lookup"><span data-stu-id="cf020-116">a.</span></span> <span data-ttu-id="cf020-117">회사 또는 학교 계정으로 [Microsoft 365에 로그인](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf020-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="cf020-118">b.</span><span class="sxs-lookup"><span data-stu-id="cf020-118">b.</span></span> <span data-ttu-id="cf020-119">왼쪽 위에서 앱 시작 관리자 아이콘을 선택하고 **관리자**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="cf020-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="cf020-120">c.</span><span class="sxs-lookup"><span data-stu-id="cf020-120">c.</span></span> <span data-ttu-id="cf020-121">왼쪽 아래 탐색에서 **관리자**를 확장하고 **Exchange**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="cf020-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="cf020-122">d.</span><span class="sxs-lookup"><span data-stu-id="cf020-122">d.</span></span> <span data-ttu-id="cf020-123">**보호**  >  **dkim**으로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf020-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="cf020-124">e.</span><span class="sxs-lookup"><span data-stu-id="cf020-124">e.</span></span> <span data-ttu-id="cf020-125">도메인을 선택 하 고 **이 도메인에 대해 DKIM 서명을 사용 하 여 서명 메시지**에 대해 **사용** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf020-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="cf020-126">각 사용자 지정 도메인에 대해 이 단계를 반복합니다.</span><span class="sxs-lookup"><span data-stu-id="cf020-126">Repeat this step for each custom domain.</span></span>
