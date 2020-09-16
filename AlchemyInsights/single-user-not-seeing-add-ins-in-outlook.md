---
title: 단일 사용자가 Outlook에서 추가 기능을 확인할 수 없는 경우
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 8c99b443a2d83f3ac24362d63cd6363a66a81393
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719671"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="f5483-102">단일 사용자가 Outlook에서 추가 기능을 확인할 수 없는 경우</span><span class="sxs-lookup"><span data-stu-id="f5483-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="f5483-103">사용자가 올바른 AppsForOfficeEnabled 매개 변수를 갖지 않는 역할의 일부일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f5483-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="f5483-104">해당 cmdlet을 실행하여 사용자에게 올바른 역할이 연결되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="f5483-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="f5483-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="f5483-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="f5483-106">자세한 내용은 [관리자 및 Outlook 추가 기능을 설치하고 관리할 수 있는 사용자 지정](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f5483-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
