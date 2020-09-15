---
title: 도메인 이동
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
- "9002570"
- "4985"
ms.openlocfilehash: 551517b99f8f725f7034efdc73e866e296dec8b6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47678762"
---
# <a name="domain-transfers"></a><span data-ttu-id="664c4-102">도메인 이동</span><span class="sxs-lookup"><span data-stu-id="664c4-102">Domain transfers</span></span>

<span data-ttu-id="664c4-103">[60 일 후에 다른 공급자에게 Microsoft 구입 도메인을 전달하는 방법](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).</span><span class="sxs-lookup"><span data-stu-id="664c4-103">[How to transfer a Microsoft purchased domain to another provider after 60 days](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).</span></span>

<span data-ttu-id="664c4-104">Microsoft에서 구입한 도메인은 NS 레코드 변경을 지원하지 않지만 도메인 등록을 웹 호스트로 전송하는 대신 [웹 사이트의 DNS 레코드 업데이트](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider?view=o365-worldwide)를 고려해 보세요.</span><span class="sxs-lookup"><span data-stu-id="664c4-104">Although Microsoft purchased domains don't support changing NS records, consider [updating DNS records for your website](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider?view=o365-worldwide) instead of transferring your domain registration to the web hoster.</span></span>

<span data-ttu-id="664c4-105">Microsoft 구입 도메인은 Microsoft 365 테넌트 간에 이전할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="664c4-105">A Microsoft purchased domain cannot be transferred between Microsoft 365 tenants.</span></span>

<span data-ttu-id="664c4-106">그러나 [한 테넌트에서 도메인을 제거](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain?view=o365-worldwide)한 다음 다른 테넌트의 도메인을 확인함으로써 Microsoft 365 테넌트 간에 타사 도메인을 이전할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="664c4-106">However, you can transfer a third-party domain between Microsoft 365 tenants by [removing the domain from one tenant](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain?view=o365-worldwide) and then verifying the domain in another tenant.</span></span>

<span data-ttu-id="664c4-107">타사 도메인 등록 또는 대금 청구를 Microsoft로 이전할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="664c4-107">A third-party domains registration or billing cannot be transferred to Microsoft.</span></span>

<span data-ttu-id="664c4-108">사용자 지정 도메인은 [Microsoft 365로 확인하고 사용](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain?view=o365-worldwide)할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="664c4-108">Custom domains can be  [verified and used with Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain?view=o365-worldwide).</span></span> <span data-ttu-id="664c4-109">Onmicrosoft.com 기본 도메인은 전송하거나 이름을 바꿀 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="664c4-109">Onmicrosoft.com default domains cannot be transferred or renamed.</span></span>
