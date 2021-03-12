---
title: Office 365 보안 및 준수 센터에서 감사 로그 역할 할당
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736850"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="47f9b-102">Office 365 보안 및 준수 센터에서 감사 로그 역할 할당</span><span class="sxs-lookup"><span data-stu-id="47f9b-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="47f9b-103">Office 365 감사 로그를 검색하려면 관리자는 **보기 전용 감사 로그** 역할이나 Exchange Online의 **감사 로그** 를할당해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="47f9b-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="47f9b-104">이러한 역할은 기본적으로 준수 관리 및 조직 관리 역할 그룹에 할당됩니다.</span><span class="sxs-lookup"><span data-stu-id="47f9b-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="47f9b-105">Office 365 및 Microsoft 365의 전역 관리자는 자동으로 조직 관리 역할 그룹의 구성원이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="47f9b-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="47f9b-106">사용자가 최소 수준의 권한으로 검색할 수 있도록 하려면 Exchange Online에서 사용자 지정 역할 그룹을 생성하고 **보기 전용 감사 로그** 역할 또는 **감사 로그** 역할을 추가한 다음 사용자를 새 역할 그룹의 구성원으로 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47f9b-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="47f9b-107">자세한 내용은 [Exchange Online에서 역할 그룹 관리](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) 및 [보안 및 준수 센터에서 감사 로그 검색](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="47f9b-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>