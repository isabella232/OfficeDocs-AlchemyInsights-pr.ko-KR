---
title: 공유 정책 및 조직 관계에 PowerShell 사용
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
ms.openlocfilehash: 48df03b1397b0e924aa878cea3d1cac07ca862c3636c1273d10f4841a03fddcf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998472"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>공유 정책 및 조직 관계에 PowerShell 사용


조직 관계에 대한 자세한 정보는 다음에 대한 자세한 구문 및 매개 변수 정보를 확인하세요. [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  및  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

공유 정책을 만들려면 [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy)를 사용하세요. [사서함 또는 사용자에 공유 정책을 적용](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)하려면 [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) 및 [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox)를 새로 만든 정책과 함께 사용해야 합니다. [공유 정책을 수정, 비활성화 또는 제거](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)하려면 [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) 및 [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)를 사용해야 합니다.

**이 항목에 대한 자세한 내용은 다음을 참조 하세요.**

[Exchange Online에서 공유](https://docs.microsoft.com/exchange/sharing/sharing)