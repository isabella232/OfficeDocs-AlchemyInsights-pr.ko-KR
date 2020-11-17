---
title: 권한 있는 Id 관리 역할
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086379"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="b51a6-102">PIM (권한 Id 관리) 역할</span><span class="sxs-lookup"><span data-stu-id="b51a6-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="b51a6-103">**역할을 활성화 한 후에 권한이 부여 되지 않음**</span><span class="sxs-lookup"><span data-stu-id="b51a6-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="b51a6-104">Azure AD PIM (권한 부여 Id 관리)에서 역할을 활성화 하면 권한 있는 역할이 필요한 모든 포털에 인증이 즉시 전파 되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="b51a6-105">변경 내용이 전파 되더라도 포털의 웹 캐싱으로 인해 변경 내용이 즉시 적용 되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="b51a6-106">정품 인증이 지연 되는 경우 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="b51a6-107">Azure portal에서 로그 아웃 한 다음 다시 로그인 하세요.</span><span class="sxs-lookup"><span data-stu-id="b51a6-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="b51a6-108">Azure AD 역할 또는 Azure 리소스 역할을 활성화 하면 정품 인증 단계가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="b51a6-109">모든 단계가 완료 되 면 ' 로그 아웃 ' 링크가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="b51a6-110">이 링크를 사용 하 여 로그 아웃할 수 있습니다. 이렇게 하면 대부분의 경우 정품 인증 지연에 대 한 해결이 실행 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="b51a6-111">PIM에서 역할의 구성원으로 나열 되어 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="b51a6-112">Exchange 관리자 역할을 활성화 하는 경우 로그 아웃 하 고 다시 로그인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="b51a6-113">문제가 계속 되 면 지원 티켓을 열고 문제를 제기 합니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="b51a6-114">Exchange 관리자 역할을 사용 하 여 보안 및 준수 센터에 액세스 하는 경우 다음 단계를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="b51a6-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="b51a6-115">보안 및 준수 센터에 액세스 하기 위해 역할을 활성화 하거나 SharePoint 관리자 역할을 활성화 하는 경우 몇 분에서 몇 시간까지 몇 가지 정품 인증 지연이 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="b51a6-116">이는 알려진 문제 이므로 가능한 한 빨리이 문제를 해결 하기 위해 이러한 팀과 협력 하 고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="b51a6-117">자세한 내용은 다음을 참조하시기 바랍니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-117">For more information, see:</span></span>

- [<span data-ttu-id="b51a6-118">PIM에서 내 Azure AD 역할 활성화</span><span class="sxs-lookup"><span data-stu-id="b51a6-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="b51a6-119">PIM에서 내 Azure 리소스 역할 활성화</span><span class="sxs-lookup"><span data-stu-id="b51a6-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="b51a6-120">**역할을 비활성화 하거나 역할 활성화가 만료 된 후에 사용 권한이 제거 되지 않음**</span><span class="sxs-lookup"><span data-stu-id="b51a6-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="b51a6-121">Azure AD 권한 있는 Id 관리에서 역할을 비활성화 하거나 역할 활성화 기간이 만료 되는 경우 계속 해 서 액세스 권한이 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="b51a6-122">비활성화가 지연 되는 경우 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="b51a6-123">Exchange 관리자 역할을 비활성화 하거나 역할 활성화 기간이 만료 되는 경우 사용 권한이 제거 되기 전에 상당한 지연이 발생 하면 지원 티켓을 열고 지원 엔지니어에 게 문의 하 여이 문제에 대해 Office 내부의 PAM (권한 부여 관리) 팀과 티켓을 파일 하는 데 도움을 주어 야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="b51a6-124">정품 인증 기간이 만료 되었지만 여전히 브라우저 세션이 열려 있으면 브라우저를 닫습니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="b51a6-125">해당 세션을 닫을 때까지이 역할을 계속 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="b51a6-126">이는 알려진 문제로, 정품 인증이 만료 된 후에 각 세션을 적극적으로 해지 하기 위해 가능한 수정 사항을 확인 하 고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b51a6-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="b51a6-127">지연 시간이 이러한 두 시나리오와 다를 경우 지원 티켓을 여십시오.</span><span class="sxs-lookup"><span data-stu-id="b51a6-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
