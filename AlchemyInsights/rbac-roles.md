---
title: 'RBAC 역할 '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576528"
---
# <a name="rbac-rules"></a><span data-ttu-id="64976-102">RBAC 규칙</span><span class="sxs-lookup"><span data-stu-id="64976-102">RBAC rules</span></span>

<span data-ttu-id="64976-103">사용 권한 오류가 발생하는 경우:</span><span class="sxs-lookup"><span data-stu-id="64976-103">If you get the permission error:</span></span> 

- <span data-ttu-id="64976-104">개체 ID가 있는 클라이언트에는 **범위(코드: AuthorizationFailed)를** 통해 작업을 수행할 수 있는 권한이 없습니다. 리소스를 만들려고 할 때 선택한 범위에서 리소스에 대한 쓰기 권한이 있는 역할이 할당된 사용자로 현재 로그인되어 있는지 확인</span><span class="sxs-lookup"><span data-stu-id="64976-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="64976-105">예를 들어 리소스 그룹에서 가상 컴퓨터를 관리하기 [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) 위해 리소스 그룹(또는 상위 범위)에 가상 컴퓨터 참가자 역할이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="64976-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="64976-106">각 기본 제공 역할에 대한 사용 권한 목록은 Azure 리소스에 대한 기본 제공 역할을 [참조하세요.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="64976-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="64976-107">지원 **요청을** 만들 수 있는 권한이 없습니다. 지원 티켓을 만들거나 업데이트하려고 할 때 지원 요청 참가자와 같은 Microsoft.Support/supportTickets/write 권한이 있는 역할이 [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)할당된 사용자로 현재 로그인되어 있는지 확인</span><span class="sxs-lookup"><span data-stu-id="64976-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="64976-108">더 이상 역할 할당을 만들 수 **없습니다(코드: RoleAssignmentLimitExceeded).** 역할을 할당하려고 할 때 대신 그룹에 역할을 할당하여 역할 할당 수를 줄이려고 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="64976-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="64976-109">Azure는 구독당 **최대 2,000개** 역할 할당을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="64976-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="64976-110">Azure RBAC 역할에 대한 자세한 내용은 [Azure RBAC 역할을 참조하세요.](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="64976-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
