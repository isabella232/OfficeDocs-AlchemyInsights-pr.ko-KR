---
title: 2419-사용할 수 없음 감사
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767605"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="812e1-102">통합 감사를 사용 하도록 설정할 수 없음</span><span class="sxs-lookup"><span data-stu-id="812e1-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="812e1-103">조직에 대해 통합 감사를 사용 하도록 설정 하려고 하면 다음과 비슷한 오류가 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="812e1-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="812e1-104">이 문제를 해결 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="812e1-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="812e1-105">[Exchange Online Powershell에 연결](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)합니다.</span><span class="sxs-lookup"><span data-stu-id="812e1-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="812e1-106">다음 cmdlet을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="812e1-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="812e1-107">이전 설정이 적용 되려면 60 분 정도 기다립니다.</span><span class="sxs-lookup"><span data-stu-id="812e1-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="812e1-108">Exchange Online PowerShell에서 다음 명령을 실행 합니다.</span><span class="sxs-lookup"><span data-stu-id="812e1-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="812e1-109">자세한 내용은 다음 문서를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="812e1-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="812e1-110">다단계 인증을 사용하여 Exchange Online PowerShell에 연결</span><span class="sxs-lookup"><span data-stu-id="812e1-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="812e1-111">감사 로그 검색 켜기 또는 끄기</span><span class="sxs-lookup"><span data-stu-id="812e1-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
