---
title: 구독 액세스
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/27/2020
ms.locfileid: "48773776"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="cd189-102">브라우저 문제 (브라우저 멈춤, 계속 회전, 로드 되지 않음 등)로 인해 Azure에 로그인 할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="cd189-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="cd189-103">중단으로 인해 영향을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd189-103">You might be impacted by an outage.</span></span> <span data-ttu-id="cd189-104">지속적인 중단 상태가 있는지 확인 하세요. [Azure Health Status](https://status.azure.com/status/history/)입니다.</span><span class="sxs-lookup"><span data-stu-id="cd189-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="cd189-105">모든 활성 Azure 세션에서 로그 아웃 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd189-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="cd189-106">웹 브라우저에서 비공개 또는 incognito 모드를 시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd189-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="cd189-107">또한 브라우저를 새로 고치고 다른 브라우저를 사용 하 고, 위의 경우 캐시 쿠키가 작동 하지 않는 경우에는 삭제를 시도할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd189-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="cd189-108">자세한 정보: [로그인 문제 해결](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="cd189-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="cd189-109">**구독에 액세스할 수 없음**</span><span class="sxs-lookup"><span data-stu-id="cd189-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="cd189-110">[Azure portal](https://portal.azure.com/)의 오른쪽 맨 위에 있는 계정에서 올바른 Azure 디렉터리를 선택 했는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd189-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="cd189-111">[Azure 계정 센터](https://account.windowsazure.com/Subscriptions)에서 사용 하는 계정이 계정 관리자 인지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd189-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="cd189-112">자세한 정보: [구독을 찾을 수 없는 문제 해결](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="cd189-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="cd189-113">**청구 내역에 액세스할 수 없음**</span><span class="sxs-lookup"><span data-stu-id="cd189-113">**Unable to access billing history**</span></span>

<span data-ttu-id="cd189-114">계정 관리자는 대금 청구 정보에 액세스 하는 사용자가 게스트 사용자로 Azure Active directory에 추가 [되거나 새 사용자를 삭제](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)하는 것을 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd189-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="cd189-115">사용자 [에 게 역할 할당 사용자에](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)게 전역 관리자 역할이 부여 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd189-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="cd189-116">게시 RBAC 정책을 사용 하 여 사용자에 게 대금 청구 액세스 [권한을 부여할](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd189-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="cd189-117">**권장 문서**</span><span class="sxs-lookup"><span data-stu-id="cd189-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="cd189-118">로그인 하 여 내 Azure 구독을 관리할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="cd189-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)