---
title: 공유 정책 및 조직 관계에 PowerShell 사용
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709472"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="8e2fa-102">공유 정책 및 조직 관계에 PowerShell 사용</span><span class="sxs-lookup"><span data-stu-id="8e2fa-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="8e2fa-103">조직 관계에 대한 자세한 정보는 다음에 대한 자세한 구문 및 매개 변수 정보를 확인하세요. [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  및  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="8e2fa-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="8e2fa-104">공유 정책을 만들려면 [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy)를 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="8e2fa-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="8e2fa-105">[사서함 또는 사용자에 공유 정책을 적용](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)하려면 [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) 및 [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox)를 새로 만든 정책과 함께 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8e2fa-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="8e2fa-106">[공유 정책을 수정, 비활성화 또는 제거](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)하려면 [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) 및 [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)를 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8e2fa-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="8e2fa-107">**이 항목에 대한 자세한 내용은 다음을 참조 하세요.**</span><span class="sxs-lookup"><span data-stu-id="8e2fa-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="8e2fa-108">Exchange Online에서 공유</span><span class="sxs-lookup"><span data-stu-id="8e2fa-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)