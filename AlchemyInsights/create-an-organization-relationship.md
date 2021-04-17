---
title: 사용자가 다른 조직과 공동 작업할 수 있도록 조직 관계 만들기
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
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816134"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="6604f-102">사용자가 다른 조직과 공동 작업할 수 있도록 조직 관계 만들기</span><span class="sxs-lookup"><span data-stu-id="6604f-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="6604f-103">Office 365 관리 센터 대시보드에서 **관리** > **Exchange** 로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="6604f-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="6604f-104">**조직** > **공유** 로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="6604f-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="6604f-105">**조직 공유** 에서 **새로 만들기** 를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="6604f-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="6604f-106">**새 조직 관계** 의 **관계 이름** 상자에 조직 관계의 이름을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="6604f-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="6604f-107">**공유할 도메인** 상자에 일정을 보도록 허용할 외부 Office 365 또는 Exchange 온-프레미스 조직의 도메인을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="6604f-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="6604f-108">도메인을 두 개 이상 입력하려면 도메인 이름을 쉼표로 구분합니다.</span><span class="sxs-lookup"><span data-stu-id="6604f-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="6604f-109">예: contoso.com, service.contoso.com</span><span class="sxs-lookup"><span data-stu-id="6604f-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="6604f-p102">**약속 있음/없음 일정 정보 공유 사용** 확인란을 선택하여 목록에 포함한 도메인에 대해 일정 공유를 설정합니다. 약속 있음/없음 일정 정보의 공유 수준과 약속 있음/없음 일정 정보를 공유할 수 있는 사용자를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="6604f-p102">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed. Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="6604f-112">약속 있음/없음 액세스 수준을 설정하려면 다음 중 하나를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="6604f-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="6604f-113">**약속 있음/없음 일정 정보와 시간만**</span><span class="sxs-lookup"><span data-stu-id="6604f-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="6604f-114">**약속 있음/없음 일정 정보(시간, 제목 및 위치 포함)**</span><span class="sxs-lookup"><span data-stu-id="6604f-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="6604f-115">약속 있음/없음 일정 정보를 공유할 사용자를 설정하려면 다음 중 하나를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="6604f-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="6604f-116">**조직의 모든 사람**</span><span class="sxs-lookup"><span data-stu-id="6604f-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="6604f-117">**지정된 보안 그룹**</span><span class="sxs-lookup"><span data-stu-id="6604f-117">**A specified security group**</span></span>  

<span data-ttu-id="6604f-118">**찾아보기** 를 클릭하여 목록에서 보안 그룹을 선택하고 **확인** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="6604f-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="6604f-119">**저장** 을 클릭하여 조직 관계를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="6604f-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="6604f-120">**참고:** 테넌트 간 구성은 개인 연락처에서 약속 있음/없음 조회를 지원하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="6604f-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="6604f-121">약속 있음/없음 조회를 수행하려면 연락처가 전체 주소 목록에 포함되어 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="6604f-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="6604f-122">**이 항목에 대한 자세한 내용은 다음을 참조 하세요.**</span><span class="sxs-lookup"><span data-stu-id="6604f-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="6604f-123">Exchange Online에서 조직 관계 만들기</span><span class="sxs-lookup"><span data-stu-id="6604f-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="6604f-124">Exchange Online의 조직 관계 수정</span><span class="sxs-lookup"><span data-stu-id="6604f-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="6604f-125">Exchange Online에서 조직 관계 제거</span><span class="sxs-lookup"><span data-stu-id="6604f-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
