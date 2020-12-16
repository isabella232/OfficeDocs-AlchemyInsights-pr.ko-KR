---
title: 관리자를 추가하고 관리하는 방법 - MCA FL/CL
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
- "9004114"
- "7424"
ms.openlocfilehash: f5791cb12e565cb04f7ac6bc9bb401fcca3e4e9e
ms.sourcegitcommit: dd9eb38bf9403de29f46c844cb64bc1d4c515afc
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49684001"
---
# <a name="how-to-add-and-manage-admins---mca-flcl"></a><span data-ttu-id="f6b56-102">관리자를 추가하고 관리하는 방법 - MCA FL/CL</span><span class="sxs-lookup"><span data-stu-id="f6b56-102">How to add and manage admins - MCA FL/CL</span></span>

<span data-ttu-id="f6b56-103">MCA(Microsoft 고객 계약)에 대한 청구 계정을 관리하려면 원하는 액세스 수준과 함께 다양한 역할을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f6b56-103">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="f6b56-104">이러한 역할은 리소스를 제어하는 데 도움이 되는 기본 제공 Azure 서비스 역할에 추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="f6b56-104">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="f6b56-105">**Azure Portal에서 청구 역할을 추가하는 경우:**</span><span class="sxs-lookup"><span data-stu-id="f6b56-105">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="f6b56-106">[Azure 포털](https://portal.azure.com/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="f6b56-106">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="f6b56-107">비용 관리 *+ 청구를 검색합니다.*</span><span class="sxs-lookup"><span data-stu-id="f6b56-107">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="f6b56-108">액세스 권한을 부여하려는 청구 계정, 청구 프로필 또는 송장 섹션과 같은 범위에서 IAM(액세스 제어)을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="f6b56-108">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="f6b56-109">IAM(액세스 제어) 페이지에는 해당 범위의 각 역할에 할당된 사용자 및 그룹이 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="f6b56-109">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="f6b56-110">사용자에게 액세스 권한을 부여하려면  페이지 위쪽에서 추가를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="f6b56-110">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="f6b56-111">역할 *드롭다운* 목록에서 역할을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="f6b56-111">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="f6b56-112">액세스 권한을 부여할 사용자의 전자 메일 주소를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="f6b56-112">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="f6b56-113">역할을 **할당하려면** 저장을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="f6b56-113">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="f6b56-114">사용자에 대한 액세스를 제거하려면 제거할 역할 할당이 있는 사용자를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="f6b56-114">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="f6b56-115">제거를 **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="f6b56-115">Select **Remove**.</span></span>

<span data-ttu-id="f6b56-116">**권장 문서**</span><span class="sxs-lookup"><span data-stu-id="f6b56-116">**Recommended Documents**</span></span>

- [<span data-ttu-id="f6b56-117">청구 역할 정의</span><span class="sxs-lookup"><span data-stu-id="f6b56-117">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="f6b56-118">청구 계정 역할 및 작업</span><span class="sxs-lookup"><span data-stu-id="f6b56-118">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="f6b56-119">MCA 청구 계정 시작</span><span class="sxs-lookup"><span data-stu-id="f6b56-119">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="f6b56-120">Microsoft 고객 계약에 대한 액세스 확인</span><span class="sxs-lookup"><span data-stu-id="f6b56-120">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
