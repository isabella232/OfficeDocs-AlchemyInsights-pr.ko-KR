---
title: 기본 Yammer 도메인 변경
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
- "9002662"
- "5162"
ms.openlocfilehash: 6a7215ef7187e8dc6c834470b4724692b239efd4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817989"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a><span data-ttu-id="9ce5b-102">기본/주 Yammer 도메인 변경</span><span class="sxs-lookup"><span data-stu-id="9ce5b-102">Changing the default/primary Yammer domain</span></span>

<span data-ttu-id="9ce5b-103">Yammer URL은 Yammer 네트워크의 현재 주 도메인 이름을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-103">The Yammer URL contains the current primary domain name for your Yammer network.</span></span> <span data-ttu-id="9ce5b-104">이 도메인 이름은 Office 365 또는 Azure AD에서 설정한 주 도메인 이름과 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-104">This domain name may not match the primary domain name set in Office 365 or Azure AD.</span></span> <span data-ttu-id="9ce5b-105">테넌트에 추가된 사용자 지정 도메인의 수와 Yammer가 지원되는 구성(1개의 테넌트: 1개의 네트워크 또는 1:1) 상태에 따라 동작에 차이가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-105">There are differences in behavior based on the number of custom domains added to the tenant, and whether Yammer is in a supported configuration (1 Tenant: 1 Network, or 1:1).</span></span> <span data-ttu-id="9ce5b-106">[Yammer 도메인 및 Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains)에 대한 설명서를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-106">Documentation on [Yammer domains and Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) is available.</span></span>

<span data-ttu-id="9ce5b-107">잘못된 도메인이 표시되는 가장 일반적인 이유는 여러 Yammer 네트워크가 존재하고 있기 때문이며 이들은 통합되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-107">The most common reason that you see an incorrect domain is that multiple Yammer networks exist and need to be consolidated.</span></span> <span data-ttu-id="9ce5b-108">네트워크 마이그레이션 도구를 사용하여 [단일 네트워크로 통합](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)하는 것이 중요한 첫 단계입니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-108">[Consolidating down to a single network](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) using the network migration tool is an important first step.</span></span> <span data-ttu-id="9ce5b-109">주 도메인을 설정하기 전에 이 작업을 완료하세요.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-109">Complete this before attempting to set your primary domain.</span></span>

<span data-ttu-id="9ce5b-110">**사용자 지정이 되지 않은 도메인**</span><span class="sxs-lookup"><span data-stu-id="9ce5b-110">**No custom domains**</span></span>

<span data-ttu-id="9ce5b-111">새 테넌트의 경우 테넌트의 기본 도메인(예: fabrikam.onmicrosoft.com)이 Yammer에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-111">For new tenants, the default domain (e.g. fabrikam.onmicrosoft.com) from the tenant will be used for Yammer.</span></span> <span data-ttu-id="9ce5b-112">주 도메인이 yammer.com/fabrikam.onmicrosoft.com로 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-112">The primary domain is set to yammer.com/fabrikam.onmicrosoft.com.</span></span>

<span data-ttu-id="9ce5b-113">**단일 사용자 지정 도메인**</span><span class="sxs-lookup"><span data-stu-id="9ce5b-113">**Single custom domain**</span></span>

<span data-ttu-id="9ce5b-114">Yammer는 Yammer의 주 도메인으로 테넌트에서 사용자 지정 도메인(예: fabrikam.com)을 자동으로 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-114">Yammer will automatically select the custom domain (e.g. fabrikam.com) from the tenant as the primary domain in Yammer.</span></span> <span data-ttu-id="9ce5b-115">이는 Yammer.com/fabrikam.com로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-115">It is set to yammer.com/fabrikam.com.</span></span> <span data-ttu-id="9ce5b-116">이 변경 사항은 도메인 동기화 서비스를 통해 적용되며 최대 24시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-116">This change is made by the domain sync service, and can take up to 24 hours to take effect.</span></span>

<span data-ttu-id="9ce5b-117">**다수의 사용자 지정 도메인**</span><span class="sxs-lookup"><span data-stu-id="9ce5b-117">**Multiple custom domains**</span></span>

<span data-ttu-id="9ce5b-118">Yammer는 기본 테넌트 도메인과 다른 주 도메인을 가질 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-118">Yammer can have a primary domain that is different from the default tenant domain.</span></span> <span data-ttu-id="9ce5b-119">사용자 지정 도메인이 여러 개 있기 때문에 Yammer는 사용 가능한 도메인들 중에 올바른 도메인을 추측하려 시도하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-119">Since there are multiple custom domains, Yammer does not attempt to guess the correct domain from those available.</span></span> <span data-ttu-id="9ce5b-120">사용자는 원하는 주 도메인으로 주 도메인 이름을 변경하도록 요청하는 지원 사례를 열어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-120">You need to open a support case to request that the primary domain name is changed to the primary domain of your choice.</span></span>

<span data-ttu-id="9ce5b-121">**추가 문제 해결 정보**</span><span class="sxs-lookup"><span data-stu-id="9ce5b-121">**Additional troubleshooting information**</span></span>

<span data-ttu-id="9ce5b-122">경우에 따라 테넌트 간에 도메인이 이동되어 도메인 동기화 서비스를 성공적으로 실행할 수 없었을 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-122">In some cases domains may have been moved between tenants and the domain sync service has not been able to run successfully.</span></span> <span data-ttu-id="9ce5b-123">사용자에게 잘못된 주 도메인 외에 로그인 또는 기타 문제가 발생할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-123">You may experience sign-in or other issues, in addition to an incorrect primary domain.</span></span> <span data-ttu-id="9ce5b-124">이 문제를 해결하기 위해 Microsoft 지원의 도움을 받아 도메인을 올바른 네트워크로 이동해야 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-124">To resolve this problem, domains may need to be moved to the correct network with help from Microsoft Support.</span></span> <span data-ttu-id="9ce5b-125">이러한 상황에서는 직접적인 도움이 필요하며, 문제를 해결하는데 시간이 다소 걸릴 수 있습니다(특히 도메인 이름 목록이 아주 긴 경우).</span><span class="sxs-lookup"><span data-stu-id="9ce5b-125">This situation requires direct assistance and can take some time to resolve, especially if there is a very long list of domain names.</span></span> <span data-ttu-id="9ce5b-126">지원 사례를 열고 이러한 유형의 문제를 해결하는 데 도움을 받도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-126">Open a support case to get assistance with resolving these types of issues.</span></span>

<span data-ttu-id="9ce5b-127">지원 에이전트를 이용하여 작업하는 경우, 도메인이 사용자의 제어 하에 테넌트에서 도메인이 확인되는지 검사를 진행할 것입니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-127">When working with a support agent, they will check that domains are verified on a tenant under your control.</span></span> <span data-ttu-id="9ce5b-128">에이전트는 테넌트에 추가되었지만 DNS에서 확인되지 않는 경우, 도메인에 대한 추가 확인 질문을 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9ce5b-128">They may ask additional verification questions about your domains if they are added to your tenant but not verified by DNS.</span></span> <span data-ttu-id="9ce5b-129">도메인이 DNS에서 확인되는지 확인하여 프로세스의 속도를 높일 수 있도록 합니다..</span><span class="sxs-lookup"><span data-stu-id="9ce5b-129">Please ensure that domains are verified by DNS to speed up the process.</span></span>
