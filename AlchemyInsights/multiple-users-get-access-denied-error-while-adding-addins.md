---
title: Outlook에서 추가 기능을 추가하는 동안 여러 사용자가 액세스 거부 오류가 발생합니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45397720"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="b3060-102">Outlook에서 추가 기능을 추가하는 동안 여러 사용자가 액세스 거부 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="b3060-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="b3060-103">조직에서 Outlook의 추가 기능을 설치하고 관리할 수 있는 권한을 가진 관리자를 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3060-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="b3060-104">또한 조직에서 자체 사용을 위해 추가 기능을 설치하고 관리할 수 있는 권한을 가진 사용자를 지정할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3060-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="b3060-105">자세한 내용은 [Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)에 대한 추가 기능을 설치하고 관리할 수 있는 관리자 및 사용자 지정을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="b3060-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="b3060-106">사용자에 대한 사용 권한을 성공적으로 할당했는지 확인하려면 <Role Name>을(를) 확인할 역할 이름으로 바꾸고 Exchange Online PowerShell에서 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="b3060-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="b3060-107">Get-ManagementRoleAssignment -role "<Role Name>" -GetEffectiveUsers입니다.</span><span class="sxs-lookup"><span data-stu-id="b3060-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="b3060-108">이 예에서는 조직에 대해 Office Store에서 추가 기능을 설치하기 위해 누구에게 권한을 할당했는지 확인하는 방법을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="b3060-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="b3060-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="b3060-109">PowerShell</span></span>

<span data-ttu-id="b3060-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="b3060-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="b3060-111">Get-ManagementRoleAssignment 결과에서 유효 사용자 열의 항목을 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="b3060-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="b3060-112">구문과 매개 변수에 대한 자세한 내용은 [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)를 참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="b3060-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 