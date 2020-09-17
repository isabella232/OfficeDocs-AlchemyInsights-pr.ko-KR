---
title: deflectTransport 규칙에 대 한 929 받은 편지함 규칙
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: abb729c40fb87bcca8cc03c95aa4677597d20c08
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778697"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="75ca9-102">메일 흐름 규칙 (전송 규칙이 라고도 함)</span><span class="sxs-lookup"><span data-stu-id="75ca9-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="75ca9-103">메일 흐름 규칙에 대 한 일반적인 개요: [Exchange Online의 메일 흐름 규칙 (전송 규칙)](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="75ca9-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="75ca9-104">메일 흐름 규칙 설정: [Exchange Online의 메일 흐름 규칙 절차](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="75ca9-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="75ca9-105">메일 흐름 규칙 만들기, 수정 및 삭제: [메일 흐름 규칙 관리](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="75ca9-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="75ca9-106">Exchange Online PowerShell에서 메일 흐름 규칙을 관리할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75ca9-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="75ca9-107">자세한 내용은 [Get-new-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (보기), [new-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (만들기), [제거-New-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (삭제), [설정-new-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (기존 수정), [disable-New-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (기존 항목 사용 안 함) 및 [enable-new-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (사용 하지 않도록 설정)을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="75ca9-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="75ca9-108">추가 메일 흐름 규칙 cmdlet: [get-transportruleaction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (사용 가능한 작업 나열), [get-get-transportrulepredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (사용 가능한 조건 및 예외 목록), [내보내기-export-transportrulecollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (규칙 내보내기) 및 [가져오기-export-transportrulecollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (가져오기 규칙)</span><span class="sxs-lookup"><span data-stu-id="75ca9-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
